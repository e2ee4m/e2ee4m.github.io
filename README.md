# E2EE for Mail

The Protocol 
- Scenario:
  - foo@abc.com needs to send email to bar@xyz.com
  - foo, bar, abc.com, xyz.com are just examples
- Assumptions:
  - abc.com has Foo's public key coz Foo is a user there (and only Foo has his private key)
  - xyz.com has Bar's public key coz Bar is a user there (and only Bar has his private key)
- Steps:
  - abc.com sends xyz.com Foo's public key (so Bar can reply)
  - abc.com asks xyz.com for Bar's public key (so abc.com can encrypt on client side)
  - abc.com client (software or in browser) encrypts Foo's email and send just as classic email
  - xyz.com client (software or in browser) decrypts the email and show to Bar
  - Bar reads and may reply with the same process
