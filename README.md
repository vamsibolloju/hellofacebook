hellofacebook
=============

 "hellofacebook" is an angular service provider.
 This sercice perovides two methods "login" and "logout" for facebook in our application.
 
 
Install
=============
  
  ###Bower package
  
   Bower install hellofacebook

#Usage
'''
 var app = angular.module("sampleapp" , [ "hellofacebook"  ]) 
 function  sampleCtrl( $scope , hellofacebook ){
     $scope.facebooklogin = function(){
       hellofacebook.login().then(function(success){
       },function(err){
       })
     };
     $scope.facebooklogout = function(){
         hellofacebook.logout();
     }
 }
'''
