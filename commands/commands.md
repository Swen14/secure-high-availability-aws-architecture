# Commands Used in the Project

## 1. Login to Bastion Host

```bash
ssh -i project-2.pem ubuntu@<BASTION_PUBLIC_IP>
```

Purpose:
Connect to the Bastion Host instance located in the public subnet.

---

## 2. Login to Private EC2 Instance from Bastion Host

```bash
ssh ubuntu@<PRIVATE_INSTANCE_PRIVATE_IP>
```

Purpose:
Access the EC2 instance located in the private subnet through the Bastion Host.

---

## 3. Navigate to Working Directory

```bash
cd ~
```

Purpose:
Move to the home directory before creating application files.

---

## 4. Create and Edit HTML File Using Vim

```bash
vim index.html
```

Purpose:
Create and edit the web page content.

---

## 5. Add HTML Content

```html
<h1>AWS Project to Demonstrate Apps in Private Subnet</h1>
```

Purpose:
Create a simple web page to verify application accessibility.

---

## 6. Save and Exit Vim

```text
ESC
:wq
```

Purpose:
Save changes and exit the Vim editor.

---

## 7. Start Python HTTP Server

```bash
python3 -m http.server 8000
```

Purpose:
Launch a lightweight web server on port 8000 to serve the HTML page.

---

## 8. Verify Application Access

Access the application through the Application Load Balancer DNS name:

```text
http://<LOAD_BALANCER_DNS_NAME>:8000
```

Purpose:
Verify that requests are successfully routed from the Load Balancer to the application running on the private EC2 instance.

---

## 9. Exit Private Instance

```bash
exit
```

Purpose:
Close the private EC2 session and return to the Bastion Host.

---

## 10. Exit Bastion Host

```bash
exit
```

Purpose:
Close the Bastion Host session.
