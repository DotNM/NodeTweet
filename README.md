# NodeTweet
EchoIRLP NodeTweet - Add-on for amateur radio EchoLink and IRLP nodes to make the node tweet when other nodes or users connect/disconnect from the EchoLink/IRLP node


# Requirements
You must have a working instance of EchoIRLP on your node.


# Installation

1.  Download all the files and save them to /nodetweet on your IRLP node
2.  Run the follwing commands:
	chown repeater:repeater /nodetweet/*
	chmod 755 /nodetweet/*.php
3.  Edit the nodetweet.php file to include your Twitter API keys (see http://api.twitter.com/)
4.  Add the following line to /home/irlp/custom/custom_on:
	php /nodetweet/nodetweet.php -aC 
5.  Add the following line to /home/irlp/custom/custom_off:
	php /nodetweet/nodetweet.php -aD
