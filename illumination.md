- First we download and unzip the file, we will see the hidden folder called .git.

![image](https://user-images.githubusercontent.com/111954330/200496502-bf33f50e-61aa-4ff6-89eb-c15cc0df6714.png)

- All the history of changes by dev are stored in the log portion.
- We use “git log” to show all the changes.

![image](https://user-images.githubusercontent.com/111954330/200496522-f885311e-8a45-42ff-85fc-1879240a0230.png)

- We should focus on the one with the removed token which is the 2nd one.
- Use “git show 47241a47f62ada864ec74bd6dedc4d33f4374699” to see it with more details.

![image](https://user-images.githubusercontent.com/111954330/200496551-cbded358-6d65-4612-927e-c255316e3636.png)

- We can see the token which has been removed
- Looks like it’s base64, let’s decode it

![image](https://user-images.githubusercontent.com/111954330/200496579-9bb882ff-2d83-4dfa-8795-7baf5f7321aa.png)

- We get the result:
<h1>HTB{v3rsi0n_c0ntr0l_am_I_right?}<h1>
