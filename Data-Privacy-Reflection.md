# Data Privacy Reflection

## Research & Learn

### Key takeaways from Focus Bear's privacy policy
Focus Bear collects different categories of data depending on what a user does in the app, such 
as identification data (email, login), habit and lifestyle data (double encrypted so only the 
user can see it), technical data (device and OS info), payment data (handled securely through 
Stripe, not stored directly by Focus Bear), and in some cases special category data like health 
or religious information if a user's habits or optional survey answers reveal it (for example, an 
ADHD survey question). Focus Bear follows GDPR rules, only keeps data as long as necessary, and 
works with trusted third party services like Auth0, AWS, and Cloudflare to keep data secure. Users 
also have rights like accessing, correcting, or deleting their data at any time.

### What types of data are considered confidential at Focus Bear?
User identification details (email, login credentials), habit and lifestyle data, health related 
information (such as ADHD or autism survey answers), payment details, and any internal company 
data such as credentials, tokens, or internal documents.

### What are best practices for handling confidential data?
Never sharing sensitive data outside of approved tools, using strong passwords and 2FA, encrypting 
sensitive data where possible, only accessing data that is necessary for the task at hand, and 
not storing confidential information in unsecured places like personal notes or public 
repositories.

### How should you respond to a suspected data breach or accidental disclosure of confidential information?
Report it immediately to a supervisor or the relevant team, avoid trying to hide or fix it alone, 
change any potentially compromised passwords or tokens right away, and follow the company's breach 
response process instead of staying silent about it.

## Reflection

### What steps can you take to ensure you handle data securely in your daily tasks?
Avoiding putting real tokens, passwords, or personal user data into files that get pushed to 
public repositories, using environment files that are excluded from version control (like .env 
with .gitignore) for sensitive credentials, and double checking before sharing any data outside 
the team.

### How should you store, share, and dispose of sensitive information safely?
Store sensitive information in secure, access controlled places, share it only through approved 
and secure channels, and dispose of it by properly deleting files rather than just leaving them 
in random folders once they are no longer needed.

### What are some common mistakes that lead to data privacy issues, and how can they be avoided?
Common mistakes include accidentally committing secrets or tokens into a public GitHub repository, 
reusing weak passwords, or sharing sensitive data over unsecured channels. These can be avoided 
by using .gitignore for sensitive files, using a password manager, and double checking what is 
being shared and where before sending it.

## Task

### One habit or practice to improve data security in my role
I will always check my .env files and any config files for sensitive tokens or credentials before 
committing code, and make sure they are listed in .gitignore so they never get pushed to a public 
repository.

### One key learning or security measure I will implement
I learned that Focus Bear double encrypts sensitive user data like habits, so only the user can 
see it. This showed me the importance of encrypting or protecting sensitive data even internally, 
not just relying on access permissions. Going forward, I will be more careful about never 
hardcoding secrets directly into code and always using environment variables instead.