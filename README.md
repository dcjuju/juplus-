#juPlus
A google+ plugin that will easily allow you to fetch user information or basic data profile from google+ .

##Include to your page
Include jquery and juPlus plugin into your page.

```
<script src="https://code.jquery.com/jquery-2.2.1.min.js"></script>
<script src="https://rawgit.com/dcjuju/juplus/master/juplus.min.js"></script>
```

##Usage
```
$.juplus({
  options : value,
  ...
})
```
###Options
| Option        | Description           |
| ------------- |:-------------:|
| id     | required option, your google+ client id  |
| email     | the email of the user, the email will be set as a value of the given input  |
| firstname     | the firstname of the user, the firstname will be set as a value of the given input  |
| lastname     | the lastname of the user, the lastname will be set as a value of the given input  |
| fullname     | the fullname of the user, the fullname will be set as a value of the given input  |
| imageUrl     | the profile image url of the user, the url will be set as a source attribute  |
| googleId     | the googleId of the user, the googleId will be set as a value of the given input  |
##Example
###Html
>id option is required it will throw an error if you didnt specify it 
```
<input type="text" id="email"/>
<img src="" id="myimage"/>
```
###JS
```
$.juplus({
  id: 'mygoogleclientid',
  email : '#email',
  imageUrl: '#myimage'
})
```
>Make sure to include jquery first before the juplus plugin
