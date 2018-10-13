# Thought Note

_This is a dumping ground for all the random thoughts that I have that needs to be organize first._

## TODO
- research XMPP & Firebase cloud messaging
	- From my understanding MQTT & websocket are too low-level for me right now

Ultimately I think actually having a database makes the most sense
- The point of this product is "1 stop shop" for flat sharing, and it should strive to make everything as easy to use as possible
- Respecting people's privacy + GDPR is not impossible. Thousands if not millions of companies are doing it already
- All I need is to not have table/column/etc that is personal identifyable by design
	- message is the only "exception" because you can't control what the user write
- Message should be XMPP first + a REST endpoint to fetch existing messages
- shopping list, share notes, share schedule, etc are all just standard REST endpoints
- Share file = rest endpoint + some kind of 1 time url to fetch it
	- Even if you intercepted the url, you won't be able to download it
- user verification
	- it should be essentially 2fa for every request
		- when sign up, both side share a secret
		- for every request, it takes a user id + passphrase (which changes super regularly)
			- user id is needed to 

i want the joining process easy for both sides
-> i don't want to force user to get a printer or something
-> i don't want user to enter a long string of character

- It kinds has to be number based
- The best I can do is "0123456789." 11 different char
	- For now it can be 11^9 = 2357947691
- User can just write it down on a post-it note pretty easily 
- "We will let you know the moment when your roommate confirmed you just moved in (jazz hands emoji)"


Authentication

- After you have been approved, the new user receives token (Push notification maybe? Still TBC esp. the security part) that last forever
- Every request needs to use that token
- It should be revoke-able, but that's not urgent at this moment
