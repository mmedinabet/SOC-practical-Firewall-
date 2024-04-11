<h1> Security Operations Center Practical #1: Firewall configuration</h1>

The website at 203.0.110.1 is under attack! Quickly add some firewall rules to stop the server from crashing!
The packets in red are from the attacker's machine!

![1Screenshot 2024-04-11 1 21 29 PM](https://github.com/mmedinabet/SOC-practical-Firewall-/assets/142737434/2a8fad1c-5131-4f06-b13a-3d5eb1dfd05f)

To effectively block the ongoing attack at the firewall level, we need to create firewall rules that deny traffic from the malicious IP address to all destination ports. Since the attack appears to target various destination ports with malicious packets, we'll set the destination port as "ANY" to cover all ports. The action will be set to "DROP" to block the traffic.

Here's the firewall rule to add:

![Screenshot 2024-04-11 1 37 04 PM](https://github.com/mmedinabet/SOC-practical-Firewall-/assets/142737434/7083c9ad-5c42-4745-99aa-56f9113dcb42)


Replace "Malicious_IP_Address" with the actual IP address of the attacker.

![Screenshot 2024-04-11 1 30 08 PM](https://github.com/mmedinabet/SOC-practical-Firewall-/assets/142737434/48a0ba0a-a235-467c-bf66-34bb4e9a950b)

![5 Screenshot 2024-04-11 1 21 46 PM](https://github.com/mmedinabet/SOC-practical-Firewall-/assets/142737434/fa27332d-0d47-4f61-8e4f-4f9ecc9a3506)


After successfully stopping the attack, the flag received would typically indicate the completion or success of the task. The specific flag might vary depending on the simulation or training scenario, but it could be something like "ATTACK_STOPPED" or "TASK_COMPLETED".

![Screenshot 2024-04-11 1 32 12 PM](https://github.com/mmedinabet/SOC-practical-Firewall-/assets/142737434/363cf72f-9079-417c-9734-6726bbf1b8b7)

<h2>Conclusion</h2>

The exercise involved swiftly responding to an ongoing attack targeting the website at 203.0.110.1. By analyzing the network traffic, it was determined that the attack originated from a specific IP address, indicating a malicious actor attempting to compromise the server. To mitigate the threat and prevent the server from crashing, firewall rules were promptly implemented to block traffic from the attacker's IP address. Specifically, port 80, a common target for web traffic and potentially malicious payloads, was effectively blocked. This action helped to thwart the attack and safeguard the website from further harm. The exercise underscores the importance of proactive security measures, such as firewall configuration, in defending against cyber threats and ensuring the resilience of networked systems.
