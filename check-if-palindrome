#!/usr/bin/perl

use warnings;
use strict; 
use Unicode::Normalize;		

print "\n.......................................\n        Palindrome or Not?        \n.......................................\n
	\nPlease enter value you wish to examine. \n \n";
# This is used to prompt the user enter the string they wish to evaluate.

my $userinput = lc <STDIN>; 		# defines my $userinput variable as the user input and converts it to lowercase
	$userinput =~ s/ //g;	# removes spaces from the user input
	$userinput =~ s/	//g;	# removes tabs from the user input
	chomp ($userinput);		# helps get an accurate character count when we determine length

my $length = length ($userinput);	# determines length of the user input, $userinput

my @array = split(//, $userinput);	# defines the array @array as a series of individual characters from the user input

# this 'for' statement  sets conditions such that as long as our array variable, $i, is less that the the length of the user input, it will continue through the loop. Thus,  $i will increase from 0 > 1 > 2 etc. until reaching total length of string.
for (my $i = 0; $i < $length; $i++){			
	if ($array[$i] eq @array[$length-($i+1)]){
}

# this 'if' statement sets conditions such that if an '$i' value is not the same as the corresponding value on the opposite side of the string, it recognizes that you do not have a palindrome and will give you the 'Not a palindrome.' message.  
	if ($array[$i] ne @array[$length-($i+1)]){	
	print "\nYour input is not a palindrome.\n \n"; 
	last; 						# last stops the loops when a string does not qualify as an array
}

# this last 'if' statment sets conditions such that if the loop continues through the array and all corresponding values are equal, it will print the 'Palindromic!" message.
	if ($i eq $length-1){				
	print "\nYour input is a palindrome!\n \n";
}
	
}

