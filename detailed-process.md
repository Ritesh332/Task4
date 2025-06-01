**Here is a step-by-step guide to setting up and testing a firewall on Kali Linux.**
1.  **Check UFW Status**

    ![Command to Check ufw Status](screenshots/ufw-status.png)
    
2.  **Enable UFW**  (Use 'sudo' if you aren't a root user)
   
    ![Command to Enable ufw](screenshots/enabling-ufw.png)

3. **List Current Firewall Rules**

   ![Command To List Firewall Rules](screenshots/ufw-list.png)
   
4. **Add a Rule to Block Inbound Traffic on a Specific Port (e.g., 23 for Telnet)**
   
   ![Rule to block traffic](screenshots/ufw-deny.png)

   Trying to connect

   ![Telnet Connection Request](screenshots/telnet-connection-denied.png)

 5. **Test the Rule by Attempting to Connect to that Port when 'Allowed'**

    ![Cross-checking point 4](screenshots/telnet_connection-accepted.png)

 6. **Add Rule to Allow SSH (Port 22)**

    ![Allow ssh](screenshots/allow-ssh.png)

    To test the SSH rule, attempt to connect to your local machine via SSH:

    ![SSH conncted](screenshots/ssh-connection.png)
    You will be prompted to confirm the connection and then for the password.

 7. **Remove the Test Block Rule to Restore Original State**

    ![Command to remove rule](screenshots/rule-removed.png)
