### Exceptions

Forma orientada à objetos para lidar com erros.

1. Try
2. Throw - Disparar a Exception
3. Catch 

### Criando Exceptions

	class CustomException extends Exception 
	{
		public function errorMessage() 
		{
			$errorMsg = 'Error on line ' . $this->getLine(). 'in' . 
			$this->getFile() . ':<b>' . $this->getMessage(); . '</b> is not a valid E-mail address';
			
			return $errorMsg;
		}
	}

	$email = "someone@example.com";

	try 
	{
		if(filter_var($email, FILTER_VALIDATE_EMAIL) === FALSE) 
		{
			throw new customException($email);
		}
	}

	catch (customException $e) 
	{
		echo $e->errorMessage();
	}

	