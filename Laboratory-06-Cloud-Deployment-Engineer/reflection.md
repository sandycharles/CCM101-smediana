# Mission 6 Reflection

**1. How does writing a docker-compose.yml file make a cloud engineer's job easier compared to manually typing commands?**

Writing a Compose file lets me define the whole application in one place and deploy it with a single command. In earlier missions, I typed each docker run command by hand, which meant long commands and easy typos. With Compose, the setup is saved, repeatable, and easy to share with teammates or keep in version control.

**2. What happens if you make an indentation error (like using a Tab instead of Spaces) in a YAML file?**

YAML uses indentation to show structure, and it does not allow tabs for indentation. If I used a Tab instead of spaces, the parser would show an error and docker-compose up would fail to start anything. Even a small mistake, like misaligning a line by one space, could place a setting under the wrong service, so careful formatting matters.

**3. Why did we use environment variables (like MYSQL_PASSWORD) in the Compose file?**

Environment variables let me pass settings such as the database name, user, and password into the containers without changing the image itself. Both services need matching values so Nextcloud can log in to MariaDB. In a real deployment, I would not hardcode passwords in the file. I would use a .env file or secrets to keep them safe.

**4. How did it feel to deploy a fully functional enterprise cloud storage system (Nextcloud) in just a few minutes?**

It was surprising how fast it was. After running docker-compose up -d, the Nextcloud setup page appeared in my browser within minutes, and the "Autoconfig file detected" message confirmed it had read my database settings. Something that sounds like complex enterprise software felt almost easy once the infrastructure was written as code.

**5. How has your understanding of Cloud Computing evolved since Mission 1?**

In Mission 1, I saw the cloud mostly as online storage and services that someone else runs. Since then, I have worked with infrastructure blueprints, multiple cloud providers, containers, and data storage. Now I see the cloud as something I can build and automate with code, where tools like Docker Compose make deployments consistent and repeatable.
