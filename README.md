app =Flask ( name ) 
@app.route('/register', methods=['GET', 'POST']) 
def register(): 
if request.method == 'POST': 
name = request.form['name'] 
email = 
request.form['email'] 
password = request.form['password'] 
# Store the user data in a database or 
file return 
render_template('success.html') 
return render_template('register.html') 
if     
name == ' main ': 
app.run(host='0.0.0.0') 
• Create an templates folder and add the following two files: 
register.html and success.html. 
register.html 
<form method="post"> 
<input type="text" name="name" placeholder="Name"> 
<input type="email" name="email" placeholder="Email"> 
<input type="password" name="password" placeholder="Password"> 
<input type="submit" value="Submit"> 
</form> 
success.html 
<h2>Registration Successful</h2> 
