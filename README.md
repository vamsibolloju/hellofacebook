hellofacebook
=============

 "hellofacebook" is an angular service provider.
 This service provides two methods "login" and "logout" for facebook in our application.
 
 
Install
=============
###Bower package
```
bower install hellofacebook;
```
 This command installs hellofacebook along with hellojs ( http://adodson.com/hello.js ).


#Usage
```
var app = angular.module('sampleapp',[ 'hellofacebook'  ]);
function sampleCtrl( $scope , hellofacebook  ){

  $scope.facebookLogin = function(){
         hellofacebook.login().then(function(data){
           // success callback
         },function(err){
           // failure callback
         })

 $scope.facebooklogout = function(){
    hellofacebook.logout();
  }

}

```
