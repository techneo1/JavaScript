# JavaScript
Exception Handling

try{
	// Test statements for any JavaScript Exceptions or manually throw the exceptions
}catch(e){ // Catch the JavaScript Exception or manually throwned Exceptions
		if(e instanceof InvalidError){// Process the exception
				// e.name
				// e.message
				// e.status
		}else if(e instanceof OutOfRangeError){// Process the exception

		}else{// re-throw the exception
				throw e;
		}
}finally{
		// What to do incase of Success/Failure
}
