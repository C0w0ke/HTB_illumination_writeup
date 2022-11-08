- Use volatility to analyze the process

![image](https://user-images.githubusercontent.com/111954330/200497107-b5e5a145-b1c8-42aa-b5ba-acf8da90cdd3.png)

- Used netscan plugin to analyze the network connection and identified that process powershell is connecting to the Malicious IP address found the email. The malicious process is powershell 2752.

![image](https://user-images.githubusercontent.com/111954330/200497199-f8f56c48-7564-4de0-9440-ae398af45b02.png)

- Lets perform a filescan and see if we can find the resume file in the memory.

![image](https://user-images.githubusercontent.com/111954330/200497244-7753d899-efd1-4245-87af-10386b0b01a2.png)

- We have some hits - lets dump them out and do strings on them.

![image](https://user-images.githubusercontent.com/111954330/200497269-63552f8a-cfaf-4176-b64c-3980245c58c8.png)

- Lets do strings on the dumped files.

![image](https://user-images.githubusercontent.com/111954330/200497311-6c05871b-d696-4281-8022-c1d5a19e7929.png)
![image](https://user-images.githubusercontent.com/111954330/200497328-a92bfc35-c6ff-4b1f-85a0-7d2912ba6762.png)

- There is some data in Base 64
- Let’s use CyberChef to decode it.

![image](https://user-images.githubusercontent.com/111954330/200497349-05ac9c55-cbf9-4ebb-8dcd-6d16cea882c3.png)

- Finally we got some readable text and I can see the flag <h1>HTB{$_j0G_y0uR_M3m0rY_$}<h1> in it.

