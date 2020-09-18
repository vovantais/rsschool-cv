1. Gedeiko,Vladimir
2. My contact info:
    - number telephone:+375297818282;
    - [vk](https://vk.com/vladimir_hiadzeika).
3. I like to learn new things, I like to develop.
   I study at IT Step courses. Sociable, sociable, proactive.
	I love self-development, books, learning foreign languages, sports, active lifestyle.
4. 
I have studied and worked with:
- HTML5
- CSS3
- Sass
- JavaScript
- jQuery
- React.js
- Redax
- Node.js
- Express.js
- BEM
- Шаблонизатор Pug
- Bootstrap
- Gulp
- Git
- Avocode
- Adobe Photoshop
5. ```
   authRoute.route("/login")
   .post(async (req, res) => {
      const { Name, pwdHash } = req.body;
      const user = await Users.findOne({ Name });
      if (!user) {
         res.status(404).json("This user wasn`t found!");
      }
      const passwordResult = await bcrypt.compareSync(req.body.Password, user.pwdHash);
      if (!passwordResult) {
         res.status(401).json("This password is not correct!");
      }
      await jwt.verify(user.Token, SECRET_WORD, (err, decoded) => {
         if (err) {
            jwt.sign({
               userName: Name,
            }, SECRET_WORD,
               {
                  expiresIn: '7d',
               } 
            )
            res.status(200).json({ Token: user.Token, message: 'You login Successfully!' });
         } else {
            res.status(200).json({ Token: user.Token, message: 'You login Successfully!' });
         }
      })
   });
	export const AuthFetch = (authPayload) => (dispatch) => {
	   dispatch({
	      type: AUTH_LOGIN_FETCH,
		});
	   axios.post(`${API_URI}/login`, { ...authPayload })
	      .then(res => dispatch(AuthSuccess(res.data)))
	      .catch(err => dispatch(AuthFailure(err.data)))
		};
		export const AuthSuccess = (payload) => ({
	   type: AUTH_LOGIN_SUCCESS,
	   payload,
		});
		export const AuthFailure = (payload) => ({
	   type: AUTH_LOGIN_FAILURE,
	   payload,
		});	
 ```
6. I study at IT Step courses. I have experience with React.js,Redax, Node.js.I did various tasks on page layout. Also I used Mongo.db databases for small applications on react. I continue to study new technologies now I am getting acquainted with PHP and  databases MySql and Laravel. 
- Github https://github.com/vovantais .
7. I studied at the INSTITUTION OF EDUCATION "GRODNENSKY STATE ELECTRICAL COLLEGE NAMED AFTER IVAN SCHASTNY" at the Technical Faculty by specialties, Electrician, Car mechanic.
Now I am studying at BIP - Institute of Law, Grodno.
Specializing in jurisprudence
8. I have been studying spoken English courses since 2018 and have experience of communicating with native speakers from America and England
Yes-grodno, Spoken English.
