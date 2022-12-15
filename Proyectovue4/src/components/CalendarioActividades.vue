<template>
  <div class="containerr">
        <div class="row">

          <div class="col-4 p-5 ">
            <div class="container ">
              <div class="text-center pt-4 fs-2 fw-bold">
                Consulta Nuestro
              </div>
              <div class="text-center fs-2 pt-1 fw-bolder" id="Calendario">Horario Semanal</div>
              <div class="fs-5 pt-3">Para saber todas las actividades programadas, puedes seleccionar la fecha en la que estes interesado. <br> <br>
              Ademas puedes solicitar una cita con nuestro profesionales <br><br>
              <button type="button" class="btn btn-outline-success"  >Ver Agenda Completa</button></div>
  
            </div>
            
          </div>
          <div class="col-4 pt-5"> 


              <div class="calendar ">

              <div class="col leftCol">
              <div class="content">
                <h1 class="date">Martes<span>Diciembre 13</span></h1>
                <div class="notes">
                  <p>
                    <input type="text" value="" placeholder="Agregar nota">
                    <a href="#" title="Add note" class="addNote animate">+</a>
                  </p>
                  <ul class="noteList">
                    <li>Nueva nota<a href="#" title="Remove note" class="removeNote animate">x</a></li>
                  </ul>
                </div>
              </div>
            </div>
              </div>
          </div>
    
            <div class="col rightCol">
              <div class="content">
                <h2 class="year">2022</h2>
                <ul class="months">
                  <li><a href="#" title="Jan" data-value="1">Ene</a></li>
                  <li><a href="#" title="Feb" data-value="2">Feb</a></li>
                  <li><a href="#" title="Mar" data-value="3">Mar</a></li>
                  <li><a href="#" title="Apr" data-value="4">Abr</a></li>
                  <li><a href="#" title="May" data-value="5">May</a></li>
                  <li><a href="#" title="Jun" data-value="6">Jun</a></li>
                  <li><a href="#" title="Jul" data-value="7">Jul</a></li>
                  <li><a href="#" title="Aug" data-value="8">Ago</a></li>
                  <li><a href="#" title="Sep" data-value="9" >Sep</a></li>
                  <li><a href="#" title="Oct" data-value="10">Oct</a></li>
                  <li><a href="#" title="Nov" data-value="11">Nov</a></li>
                  <li><a href="#" title="Dec" data-value="12" class="selected">Dic</a></li>
                </ul>
                <div class="clearfix"></div>
                <ul class="weekday">
                  <li><a href="#" title="Mon" data-value="1">Lun</a></li>
                  <li><a href="#" title="Tue" data-value="2">Mar</a></li>
                  <li><a href="#" title="Wed" data-value="3">Mie</a></li>
                  <li><a href="#" title="Thu" data-value="4">Juv</a></li>
                  <li><a href="#" title="Fri" data-value="5">Vie</a></li>
                  <li><a href="#" title="Say" data-value="6">Sab</a></li>
                  <li><a href="#" title="Sun" data-value="7">Dom</a></li>
                </ul>
                <div class="clearfix"></div>
                <ul class="days">
                    
                </ul>
                <div class="clearfix"></div>
              </div>
            </div>
        </div>
  </div>
    
</template>

<script>
export default {
  name: 'CalendarioActividades',
  props: {
    msg: String,

}
}
</script>

<style scoped>

.calendar{
	
	border-radius: 4px;
	overflow: hidden;
	width: 800px;
	height: 450px;
	margin: 0 auto;
	
	
	top: 50%;
	background-color: #ffffff;
	color: #333333;
}

.calendar h1, .calendar h2{
	font-weight: 300;
	font-size: 26px;
	line-height: 28px;
	text-transform: uppercase;
	margin: 0px 0px 20px 0px;
}

.calendar h1 span{
	display: block;
}

.calendar .col{
	position: relative;
	float: left;
	height: 100%;
}

.calendar .col .content{
	padding: 40px;
}

.calendar ul{
	margin: 0px;
}

.calendar ul li{
	list-style: none;
}

.calendar .leftCol{
	width: 40%;
	background-color: #1cad4d;
}

.calendar .noteList li{
	color: #ffffff;
	margin-bottom: 10px;
}

.calendar .notes p,
.calendar .notes input,
.calendar .noteList li{
	font-weight: 300;
	font-size: 14px;
}

.calendar .notes p{
	border-bottom: solid 1px rgba(255,255,255,0.4);
}

.calendar .notes input{
	background-color:  #1cad4d;
	color: #ffffff;
	border: none;
	width: 200px;
}

.calendar .addNote,
.calendar .removeNote{
	float: right;
	color: rgba(255,255,255,0.4);
	font-weight: bold;
	margin-left: 20px;
}

.calendar .addNote:hover,
.calendar .removeNote:hover{
	color: #ffffff;
}

.calendar .addNote{
	font-size: 16px;
}

.calendar .leftCol h1{
	color: #ffffff;
	margin-bottom: 40px;
}

.calendar .rightCol{
	width: 60%;
}

.calendar .rightCol h2{
	color: #C7BEBE;
	text-align: right;
	margin-bottom: 70px;
}

.calendar .months li,
.calendar .weekday li,
.calendar .days li{
	float: left;
	text-transform: uppercase;
}

.calendar .months li a,
.calendar .weekday li a,
.calendar .days li a{
	display: block;
	color: #747978;
}

.calendar .months li a{
	font-size: 10px;
	color: #C7BEBE;
	text-align: center;
	width: 32px;
	margin-bottom: 20px;
}

.calendar .months li .selected{
	font-weight: bold;
	color: #747978;
}

.calendar .weekday li a{
	width: 55px;
	text-align: center;
	margin-bottom: 20px;
	font-size: 12px;
}

.calendar .days li{
	width: 55px;
}

.calendar .days li a{
	width: 36px;
	height: 24px;
	text-align: center;
	margin: auto auto;
	font-size: 12px;
	font-weight: bold;
	border-radius: 12px;
	margin-bottom: 10px;
	padding-top: 10px;
}


.calendar .days li a:hover{
	background-color: #54e08a;
}



.calendar .days li .event{
	color: #1a8352;
}
</style>