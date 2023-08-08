<template>
	<div class="w3-container w3-center w3-padding-24">
		<h2>Ingresa a tu cuenta</h2>
                <form action="SVIsisLogin" method="post" target="_self">
                    <!-- El form va aquí -->
                    <label for="emlEmail">
                        Tu correo electrónico: 
                        <input type="email" id="emlEmail" name="email">
                    </label>
                    
                    <br>
                    
                    <label for="pwdPassword">
                        Contraseña: 
                        <input type="password" id="pwdPassword" name="password">
                    </label>
                    
                    <br>                    <br>

                    
                    <input type="submit" value="Ingresar">
                
                </form>
	</div>
</template>

<script>
export default {
  name: 'LoginForm'
}
</script>
