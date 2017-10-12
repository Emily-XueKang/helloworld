# helloworld
A simple Hello World App in Django. Deployed in Heroku.
https://sleepy-cliffs-13634.herokuapp.com/


# LobSendLetter

Steps to run this program:

1.Unzip the package

2.Open terminal, in command line, cd into the directory of "lobsendletter"

3.(opetional)Run "mvn clean package" to generate the target jar file, I have already run maven and generated the executable jar, so this step can be skipped.

4.In cammanlin, execute lob-1.0.jar with parameters, copy and paste command as below:

    java -cp target/lob-1.0.jar SendLetter -n "Joe Schmoe" -a1 "185 Berry Street" -a2 "Suite 170" -c "San Francisco" -s CA -z 94107 -m "This is a test letter for Lob’s coding challenge. Thank you legislator."

5.More on parameters of this program: -n is the name of sender, -a1 is address line 1, -a2 is address line2, -c is city, -s is state, -z is zip code, -m is the message body, and using double quotes to embrace input strings in one parameter

6.After executing the program, there will be a url in the output, such as:
	
	letter generated successfully at: https://s3-us-west-2.amazonaws.com/assets.lob.com/ltr_536095fbbba2e9a5.pdf?AWSAccessKeyId=AKIAIILJUBJGGIBQDPQQ&Expires=1510379223&Signature=yZbSucr1k27B%2B4BvmdPydWUZ3vY%3D

click the url, and the letter will be open in web browser as a pdf page.	

