# Validator class
Validating Class for  Form submissions 

##How to Install?

You can install the package using composer by typing the command

composer require litto/validator:v1.0

##How it Works?

$rules	=	array(
							"firstName"=>"LABEL1/EMPTY",
							"lastName"=>"LABEL2/EMPTY",
							"email"=>"LABEL3/EMAIL|EMPTY",
							"website"=>"LABEL4/URL",
							"price"=>"LABEL5/NUMBER|EMPTY",
						);
		$obj	=	new Validator($rules);
		if($obj	->	validate()){
			echo "Validation Success";
		}else{
			echo $obj->getMessage();
		}

After Form submission, just initialise the validator class and pass the validate rules


