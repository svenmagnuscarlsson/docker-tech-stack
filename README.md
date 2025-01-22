# How to Set Up the Tech Stack Using Your GitHub Repository

This guide will help you set up the tech stack (PostgreSQL, Adminer, Metabase, FastAPI) using your GitHub repository. Follow these steps carefully!

---

## **Step 1: Install Docker**

Docker is like a magic box that lets us run all these tools together without installing them on your computer.

1. **Download Docker**:
   - Go to [Docker’s website](https://www.docker.com/get-started).
   - Download and install Docker for your computer (Windows, Mac, or Linux).

2. **Check if Docker is Working**:
   - Open a terminal (Command Prompt on Windows, Terminal on Mac/Linux).
   - Type `docker --version` and press Enter.
   - If you see a version number, Docker is installed correctly!

---

## **Step 2: Clone Your GitHub Repository**

1. Open a terminal (Command Prompt on Windows, Terminal on Mac/Linux) and create a folder.
   ```bash
   mkdir tech-stack
   ```
2. Navigate to the folder where you want to clone the repository. For example:
   ```bash
   cd tech-stack
   ```
3. Clone your GitHub repository:
   ```bash
   git clone https://github.com/svenmagnuscarlsson/docker-tech-stack.git
   ```
4. Navigate into the cloned repository:
   ```bash
   cd docker-tech-stack
   ```

---

## **Step 3: Check Your Files**

Make sure your repository has the following files:
- `.env`
- `docker-compose.yml`
- `Dockerfile-fastapi`
- `main.py`
- `README.md`
- `requirements.txt`

If any files are missing, add them to your repository.

---

## **Step 4: Start Everything**

Now it’s time to start all the tools!

1. Run the following command:
   ```bash
   docker-compose up -d
   ```

---

## **Step 5: Access the Tools**

1. **PostgreSQL**: Running in the background (you won’t see it directly).
2. **Adminer**: Open your browser and go to `http://localhost:8081`. Use the database credentials from the `.env` file to log in.
3. **Metabase**: Open your browser and go to `http://localhost:3000`. Follow the setup instructions to connect to the database.
4. **FastAPI**: Open your browser and go to `http://localhost:8000`. You should see `{"message": "Hello, FastAPI with PostgreSQL!"}`.

---

## **Step 6: Celebrate!**

You’ve successfully set up a tech stack with PostgreSQL, Adminer, Metabase, and FastAPI using your GitHub repository! 🎉

---

## **Troubleshooting**

- If something doesn’t work, check the logs:
  ```bash
  docker-compose logs
  ```
- Make sure Docker is running and all files are in the correct folder.

