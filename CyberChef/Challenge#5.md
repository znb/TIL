# CyberChef Challenge #5

# SPOILERS AHEAD


I'd been struggling with Challenge #5 for a while. I got to the point where I knew the output was Bzip2 compressed.
I just couldn't figure out how/why I couldn't get the plain text.

[This](https://www.reddit.com/r/securityCTF/comments/zpwyo4/help_with_cyberchef_challenge_5_ctf/) Reddit post pointed to MIME.
A little digging pointed to "Quoted Printable", so we try: 

 1. From hex
 2. From Quoted Printable
 3. Bzip2 compress


And we have our output. 

Why?

 * The hint pointed to MIME being used. This lead me to "quoted printable" to make things work between client/server
   where we might need to encode "special characters" 
 * The "=" sign in the output after "From Hex" should have been a give away to "Quoted Printable"


# THIS IS NOT GOOD ENOUGH
