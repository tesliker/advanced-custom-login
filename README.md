# Configure the eProve URL
- Navigate to /admin/config/services/advanced-custom-login
- Set the URL

# POST Request
POST {{ domain }}/user/authenticate

### HEADERS
Content-Type: application/json
Bearer: Basic {{ base64encode the username password combination separated by : }}

### BODY
{"email":"MYEMAIL","password":"MYPASSWORD"}

Example for admin:admin
Bearer: Basic YWRtaW46YWRtaW4=