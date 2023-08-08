<template>
	<div class="w3-container w3-center w3-padding-24">
		<h2>Crea tu cuenta para hacer pedidos</h2>
                <form action="SVIsisRegister" method="post" target="_self">
                    <!-- El form va aquí -->
                    
                    <label for="txtFirstName">
                        Tus nombres: 
                        <input type="text" id="txtFirstName" name="firstName">
                    </label>
                    
                    <br>
                    
                    <label for="txtLastName">
                        Tus apellidos: 
                        <input type="text" id="txtLastName" name="lastName">
                    </label>
                    
                    <br>
                    
                    <label for="nmbDocumentId">
                        Tu cédula: 
                        <input type="number" id="nmbDocumentId" name="documentId">
                    </label>
                    
                    <br>
                    
                    
                    <label for="dateBirthdate">
                        Tu fecha de nacimiento: 
                        <input type="date" id="dateBirthdate" name="birthdate">
                    </label>
                    
                    
                    
                    <br>
                    
                    <label for="txtAddress">
                        Tu dirección de entrega: 
                        <input type="text" id="txtAddress" name="address">
                    </label>
                    
                    <br>
                    
                    <label for="emlEmail">
                        Tu correo electrónico: 
                        <input type="email" id="emlEmail" name="email">
                    </label>
                    
                    <br>
                    
                    <!-- esto requiere validación de formulario
                    <label for="emlEmailConfirm">
                        Confirma tu correo electrónico: 
                        <input type="email" id="emlEmailConfirm" name="emailConfirm">
                    </label>
                    -->
                    
                    <br>
                    
                    <label for="pwdPassword">
                        Contraseña: 
                        <input type="password" id="pwdPassword" name="password">
                    </label>
                    
                    <br>
                    
                    <!-- esto requiere validación de formulario-->
                    <label for="pwdPasswordConfirm">
                        Confirma tu contraseña: 
                        <input type="password" id="pwdPasswordConfirm" name="passwordConfirm">
                    </label>
                                        
                    <br>
                    
                    <input type="submit" value="Crear mi cuenta">
                
                </form>
	</div>
</template>

<script>
export default {
  name: 'NewAccForm'
}
</script>
