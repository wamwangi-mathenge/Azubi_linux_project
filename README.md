# Linux Project

Create a Shared Document using Linux

- Create a new user called "student1" using the root privileges
- Set a password for the "student1" user when prompted

```
sudo adduser student1
```
- Repeat the above steps to create another user called "student2"

```
sudo adduser student2
```

- Demonstrate how to switch between users using the su command

```
su student1
```

```
su student2
```

- Explain the concept of different user accounts and their purposes in a multi-user Linux environment
- As the "student1" user, create a new directory called "shared" in the home directory

```
sudo mkdir shared
```

- Change the group ownership of the "shared" directory to a shared group, such as "students"

```
sudo addgroup students
```
```
sudo chown :students shared
```

- Demonstrate how to add both "student1" and "student2" to the "students" group

```
sudo usermod -aG students student1
sudo usermod -aG students student2
```

- Set the directory permissions to allow read and write access for the group
```
sudo chmod 770 shared
```
```
sudo chmod g+rw shared
```
- Explain the concept of file ownership, groups and permissions
- Open the shared document in a text editor like Vim or Nano
- Demonstrate collaborative editing by having "student1" and "student2" make simultaneous changes to the shared document using different terminal windows.
- Explain the basic functionality of the text editor, including editing, saving and exiting
- Emphasize the importance of communication and coordination when working collaboratively on Shared Files