# jquery-validation
Automate validation form with jQuery with simple step 

# Set the rule for form 
$(document).ready(function(){
        $('#signin').validate({
            rules:{
                username:{
                    required:true
                },
                password:{
                    required:true,
                    minlength:5
                }

            },
            messages:{
                username:{
                    required:"The Username field is required!"
                },
                password:{
                    required:"The Password field is required!",
                    minlength:"The Password field must contain at least 5 character!"
                }
            }
        });
    });
    
# If return true 
$.validator.setDefaults({
        submitHandler: function() {
        //ajax here
         }
});
