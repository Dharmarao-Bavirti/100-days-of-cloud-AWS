✅ Method 1: Create Key Pair via AWS Management Console

- Log in using the provided console URL.

- Ensure the region at the top right is set to **N. Virginia (us-east-1)**.

- In the console search bar, type EC2 and open the EC2 dashboard.

  <img width="1366" height="615" alt="image" src="https://github.com/user-attachments/assets/a3c3bb49-1336-43b2-803e-7013a5bc3ea2" />
  
- In the left sidebar, scroll down to **“Network & Security”** → **“Key Pairs”**.

  <img width="1366" height="615" alt="image" src="https://github.com/user-attachments/assets/b15c9e94-d23c-45f5-a603-0cae1257c681" />


- **Click** “Create key pair”.

- Fill the form:

    - Name: `datacenter-kp`

    - Key pair type: `RSA`

    - Private key file format:

        - Choose `.pem` if you will use SSH directly

        - Choose `.ppk` if you plan to SSH using PuTTY
          
    <img width="1366" height="615" alt="image" src="https://github.com/user-attachments/assets/996172a1-d3c9-4337-9177-3d9d3b27dec7" />


- Click **“Create key pair”.**

- The private key file will download automatically. Save it securely.
