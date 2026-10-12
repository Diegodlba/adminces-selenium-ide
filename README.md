# AdminCES – Registro de un nuevo usuario tester

## Nombre del escenario

**Registro de un nuevo usuario tester y verificación de su creación.**

## Precondiciones

* El usuario cuenta con acceso a internet.
* La aplicación AdminCES se encuentra disponible.
* El usuario dispone de una contraseña válida para acceder al sitio.
* El usuario dispone de credenciales válidas para iniciar sesión.
* El email utilizado para registrar al nuevo usuario no se encuentra registrado previamente en el sistema.
* La funcionalidad de registro de usuarios se encuentra disponible.

## Justificación

Este escenario permite validar el flujo principal de registro de un nuevo usuario tester en AdminCES. Se verifica el acceso al sistema, el inicio de sesión, el ingreso de los datos requeridos, la creación del usuario y la confirmación de que el nuevo registro aparece correctamente en la lista de usuarios.

## Funciones auxiliares

### 1. Ingresar al sitio (`contraseña`)

1. Abrir el navegador.
2. Acceder a la página principal de AdminCES: http://cestore.ces.com.uy/adminces/.
3. Hacer clic en el campo de contraseña.
4. Ingresar una contraseña válida.
5. Hacer clic en el botón **Ingresar**.

### 2. Iniciar sesión (`email`, `contraseña`)

1. Hacer clic en **Iniciar sesión**.
2. Hacer clic en el campo de email.
3. Ingresar el email de inicio de sesión.
4. Hacer clic en el campo de contraseña.
5. Ingresar la contraseña correspondiente.
6. Verificar que el email ingresado coincida con el valor esperado.
7. Verificar que la contraseña ingresada coincida con el valor esperado.
8. Hacer clic en el botón **Iniciar sesión**.
9. Hacer clic en **OK** en el mensaje emergente de confirmación.
10. Verificar que el nombre del usuario autenticado se muestre correctamente.

### 3. Registrar un usuario nuevo (`nombre`, `apellido`, `email`, `país`, `contraseña`)

1. Hacer clic en **Crear usuario**.
2. Hacer clic en el campo Nombre e ingresar el nombre del usuario.
3. Hacer clic en el campo Apellido e ingresar el apellido del usuario.
4. Hacer clic en el campo Email e ingresar el email del usuario.
5. Hacer clic en el campo País de nacimiento y seleccionar el país deseado.
6. Hacer clic en el campo Contraseña e ingresar la contraseña de la nueva cuenta.
7. Marcar el checkbox correspondiente al tipo de tester.
8. Verificar que el nombre ingresado coincida con el valor esperado.
9. Verificar que el apellido ingresado coincida con el valor esperado.
10. Verificar que el email ingresado coincida con el valor esperado.
11. Verificar que el país seleccionado coincida con el valor esperado.
12. Verificar que la contraseña ingresada coincida con el valor esperado.
13. Hacer clic en el botón **Registrar**.
14. Hacer clic en **OK** en el mensaje emergente de confirmación de creación del usuario.

### 4. Cerrar sesión

1. Hacer clic en el menú desplegable del usuario, ubicado en la esquina superior de la pantalla.
2. Seleccionar **Cerrar sesión**.
3. Hacer clic en **OK** en el mensaje emergente de confirmación.

## Guion del escenario

**Escenario:** Registrar un nuevo usuario tester y verificar su creación.

1. Ingresar al sitio utilizando una contraseña válida.
2. Iniciar sesión con las siguientes credenciales:

   * **Email:** `yaniscorrea@gmail.com`
   * **Contraseña:** `12345`
3. Registrar un nuevo usuario con los siguientes datos:

   * **Nombre:** `Diego`
   * **Apellido:** `de la Barrera`
   * **Email:** `diegodlba@cestester.com`
   * **País:** `Uruguay`
   * **Contraseña:** `12345`
   * **Tipo de usuario:** Tester
4. Hacer clic en el botón **Ver usuarios**.
5. Verificar que el email `diegodlba@cestester.com` aparezca en la lista de usuarios.
6. Cerrar sesión.

## Resultado esperado

* El acceso al sitio y el inicio de sesión se completan correctamente.
* El sistema permite ingresar los datos del nuevo usuario.
* El registro del usuario tester se realiza correctamente y se muestra el mensaje de confirmación correspondiente.
* El nuevo usuario aparece en la lista de usuarios con el email registrado.
* El cierre de sesión se completa correctamente.
