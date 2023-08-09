<template>
	<div class="w3-container w3-center w3-padding-24">
		<h2>Crea tu cuenta para hacer pedidos</h2>
		<form id="account-creator" @submit.prevent="saveacc">
			<!-- El form va aquí -->
			
			<label for="first_name">
				Tus nombres: 
				<input type="text" id="first_name" name="first_name" v-model="first_name" />
			</label>
			
			<br>
			
			<label for="last_name">
				Tus apellidos: 
				<input type="text" id="last_name" name="last_name" v-model="last_name" />
			</label>
			
			<br>
			
			<label for="document_id">
				Tu cédula: 
				<input type="number" id="document_id" name="document_id" v-model="document_id" />
			</label>
			
			<br>
			
			
			<label for="birthdate">
				Tu fecha de nacimiento: 
				<input type="date" id="birthdate" name="birthdate" v-model="birthdate" />
			</label>
			
			
			
			<br>
			
			<label for="address">
				Tu dirección de entrega: 
				<input type="text" id="address" name="address" v-model="address" />
			</label>
			
			<br>
			
			<label for="email">
				Tu correo electrónico: 
				<input type="email" id="email" name="email" v-model="email" />
			</label>
			
			<br>
			
			<!-- esto requiere validación de formulario
			<label for="emlEmailConfirm">
				Confirma tu correo electrónico: 
				<input type="email" id="emlEmailConfirm" name="emailConfirm">
			</label>
			-->
			
			<br>
			
			<label for="password">
				Contraseña: 
				<input type="password" id="password" name="password" v-model="password" />
			</label>
			
			<br>
			
			<!-- esto requiere validación de formulario
			<label for="pwdPasswordConfirm">
				Confirma tu contraseña: 
				<input type="password" id="pwdPasswordConfirm" name="passwordConfirm">
			</label>
			-->
			<br>
			
			<button type="submit" id="saveacc" name="saveacc">Crear mi cuenta</button>
		
		</form>
	</div>
</template>

<script>
// importar axios
import axios from "axios";
export default {
	// el nombre del componente
	name: 'NewAccForm',
	// los datos
	data() {
		return {
			document_id: "",
			first_name: "",
			last_name: "",
			birthdate: "",
			email: "",
			password: "",
			address: "",
		};
	},

	// los metodos a manejar con axios
	methods: {
		saveacc() {
			axios.post("http://localhost:8080/api/accounts", {
				document_id: this.document_id,
				first_name:  this.first_name, 
				last_name: this.last_name,
				birthdate: this.birthdate,
				email: this.email,
				password: this.password,
				address: this.address,
			})
			.then((response) => {
				console.log("account successfully created: ", response.data);
				alert("At_id: this.document_id, account created");
				this.document_id = ''; 
				this.first_name = ''; 
				this.last_name = '';
				this.birthdate = '';
				this.email = '';
				this.password = '';
				this.address = '';
			})
			.catch((error) => {
				console.error("error when creating account: ", error);
			});
		}
	}
};
</script>
