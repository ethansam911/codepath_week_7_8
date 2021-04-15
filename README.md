# Week 9 of CodePath Cybersecurity Write-Up 

### **Unit 9**

### Milestone 0: Kali Gone Wild 

- [x] Completed

### Milestone 1: Hello, SET  ( [x] )

* Throwaway email: test user  
  * testusercodepath@gmail.com

![alt text](https://github.com/ethansam911/codepath_week_7_8/blob/main/milestone_1_google_block.png)
- Turn on Less Secure Apps for throwaway account 

https://myaccount.google.com/u/3/lesssecureapps?pli=1&rapt=AEjHL4MtX1AzjGSkoesbiFvul52AlBZcYqJatqPToyPyXGTnvcRIscLYLTldW7WmECMlBZ3ibqBRwsb1WyyFirQBZWNBtw2HaA 


![alt text](https://github.com/ethansam911/codepath_week_7_8/blob/main/milestone_1_email_sent.png)

### Milestone 2: Try a Real Payload ( [x] )

- Completed

### Milestone 3: Fakebook 

![alt text](https://github.com/ethansam911/codepath_week_7_8/blob/main/milestone_3_we_got_a_hit.png)

### Milestone 5: Clean Up

![alt text](https://github.com/ethansam911/codepath_week_7_8/blob/main/milestone_5_turn_on_nat.png)


### Milestone 6: SE In Situ

In the cases, we see a user compromised through techniques that exploit security measures partially beyond his or her control. Challenge questions:

- What vulnerabilities were beyond the control of the user?
  - Nature of the of the underlying program has a vulnerability allowing the manipulation of data.    
- What if anything could have been done by the user to mitigate the severity of the attack?
  - The user could set up 2FA and provision his account with additional security details.

Now, think back to the fake Facebook login scenario above. Assuming a successful compromise, in which the user's Facebook username and password were successfully intercepted, answer the following:

- What could the user do to mitigate this, making a successful login impossible for the attacker even with the credentials? (Hint: FB offers this as an option; not all sites do)
  - Use a third-party code generator, or receieve a nonce to authenticate the user. 
- Why might the username/password still be of value to the attacker even if she can't use them to login to Facebook? (Hint: think about how users come up with passwords)
  - Users often use the same password or similar passwords for their accounts, knowing one password could allow a threat actor to guess another password.  

