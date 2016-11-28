+++
date = "2016-08-07T20:09:19Z"
draft = false
title = "Contacto"

+++

<div id='crmWebToEntityForm'>
<META HTTP-EQUIV ='content-type' CONTENT='text/html;charset=UTF-8'>

<form action='https://crm.zoho.com/crm/WebToLeadForm' 
	name=WebToLeads2015827000000104023 method='POST' 
	onSubmit='javascript:document.charset="UTF-8"; return checkMandatory()' 
	accept-charset='UTF-8'>

	 <!-- Do not remove this code. -->
	<input type='text' style='display:none;' name='xnQsjsdp' value='670cbb754cef376380a8265570fb68c7df5f3e6204d431b7146d5bccf526d56b'/>
	<input type='hidden' name='zc_gad' id='zc_gad' value=''/>
	<!-- <input type='text' style='display:none;' name='xmIwtLD' value='d34dc902754bbad7bfd1b82d9ff6391147850e633327dc0168830469c459c195'/> -->
	<input type='text' style='display:none;' name='xmIwtLD' value='d34dc902754bbad7bfd1b82d9ff639116ed04a606f9816fe2a3471b654886c1c'/>
	<input type='text' style='display:none;'  name='actionType' value='TGVhZHM='/>

	<input type='text' style='display:none;' name='returnURL' value='http&#x3a;&#x2f;&#x2f;tigoctm.com' /> 
	 <!-- Do not remove this code. -->

  <div class="form-row">
    <label for="firstname">Nombre
      <span class="form-error" id="error-name">Favor de ingresar su nombre</span>
    </label>
    <div class="form-half-row" style="padding-right: 2%">
      <input type="text" maxlength="40" name="First Name" id="firstname"
          placeholder="Nombre">
    </div>
    <div class="form-half-row">
      <input type="text" maxlength="80" name="Last Name" id="lastname"
          placeholder="Apellido">
    </div>
  </div>

  <div class="form-row">
    <input type="text" maxlength="100" name="Email" id="email"
    	   placeholder="Email">
    <span class="form-error" id="error-email">
		Por favor especifique su email para saber como podemos comunicarnos con usted
    </span>
  </div>

  <div class="form-row">
    <label for="company">Empresa <span class="contact-info">optional</span></label>
    <input type="text" maxlength="100" name="Company" id="company">
  </div>

  <div class="form-row">
    <label for="shipping">Envío <span class="contact-info">opcional</span></label>
    <div class="form-half-row" style="padding-right: 2%">
    	 <input type="text" maxlength="80" name="Country" id="country"
          	placeholder="País">
     </div>
     <div class="form-half-row">
      <input type="text" maxlength="40" name="City" id="city"
          placeholder="Ciudad">
  </div>

  <div class="form-row">
    <label for="message">Mensaje
    <span class="form-error" id="error-message">
		Necesitaremos cierta información necesaria para poder ayudarlo mejor.	
    </span>
    </label>
    <textarea name="Description" id="message" cols="40" rows="10" maxlength="1000"></textarea>
   </div>

  <div class="form-align">
    <input type="submit" value="Solicite mayor información">
  </div>
</div>

  <script>
    var fields = ['firstname', 'lastname', 'email', 'message', 'city', 'country'];
    var basicEmail = /^[^ @]+@([^ @]+){2,}\.([^ @]+){2,}$/;

    function checkMandatory() {
      /* Hide any errors. */
      var allErrors = document.getElementsByClassName('form-error');
      for (var i = 0; i < allErrors.length; i++) {
        allErrors[i].style.display = 'none';
      }

      /* Validate the form. */
      var form = document.forms['WebToLeads2015827000000104023'];
      for (var i = 0; i < fields.length; i++) {
        var fieldObj = form[fields[i]];
        if (fieldObj) {
          var failed = fieldObj.value.replace(/^\s+|\s+$/g, '').length === 0;
          if (!failed && fields[i] === 'email') {
            failed = !basicEmail.test(fieldObj.value);
          }

          if (failed) {
            fieldObj.focus();
            var name = fields[i];
            if (name.endsWith('name')) {
              name = 'name';
            }
            var err = document.getElementById('error-' + name);
            if (err) {
              err.style.display = 'block';
            }
            return false;
          }
        }
      }
    }
  </script>
<form>
</div>
