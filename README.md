codesample-6-2013
=================







The  code sample is more difficult for me.  The most recent code I have written is proprietary cobol code owned by the University of Washington.  Since I worked supporting student systems including financial aid, unless we have a valid student id we cannot access data as it is also private.  Because I no longer work for the university due to the recessionary budget cuts imposed by the legislature, I do not have access either.  I have written programs and code to access the data requested from the mainframe but, I have not learned web development.  In an effort to give you something, I am providing you with a simple design plan to access the database and return data to be used in a web page in the attachment.  I hope this will suffice.


Data Retrieval plan for use in Web Page:

*  Identify data fields needed
*  Map needed fields to the database
*  Define edits
*  Define record to be received and returned

*  Write the cobol program using standard constructs:

	*  set up working storage
	*  open files
	*  Start the procedure section which will 
		open and read the input file 
           	determine if the request is inquiry or update 
		if update, perform any necessary edits 
           	access the database
		if update, move data and update the database
		if inquiry,  move data
 		format and write the output file 
		close files

*  Write the job control language which includes XML conversion.
	
