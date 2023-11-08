# 2. Groups

<div align="center">
  <img src="./assets/images/groups_cover.jpg" width="100%">
</div>

---

---

## Outline

#### 2.1 Create Group

#### 2.2 Modify Group

#### 2.3 Delete Group

#### 2.4 Assign user to Primary and Secondary group

#### 2.5 List all members in group

#### 2.6 Remove members from group

---

## Types of Groups in Linux System

#### 1. Primary Group

**_A primary group is automatically created when a user with a unique user ID is created._**

#### 2. Secondary Group

**_A secondary group is created by using commands. You can change the group IDs of the users and add them to this group later._**

### Login defines variables

**`cat /etc/login.defs`**

<div align="center">
  <img src="../Users/assets/images/UID&GID.png" width="100%">
</div>

### Groups stored in group file

**`cat /etc/group`**

<div align="center">
  <img src="./assets/images/etc_group.png" width="100%">
</div>

### Group passwords stored in passwd file

**`cat /etc/shadow`**

<div align="center">
  <img src="./assets/images/etc_gshadow.png" width="100%">
</div>

---

## Create User

**`groupadd GROUP_NAME`**
**`groupadd --help`**

<div align="center">
  <img src="./assets/images/groupadd_help.png" width="100%">
</div>

<br >

**`groupadd user1`**

<div align="center">
  <img src="./assets/images/groupadd_group1.png" width="100%">
</div>

---

---

## Modify Group info

**`groupmod OPTION GROUP_NAME`**
**`groupmod --help`**

<div align="center">
  <img src="./assets/images/groupmod_help.png" width="100%">
</div>

<br>

**`groupmod -g 1111 group1`**

<div align="center">
  <img src="./assets/images/groupmod_group1.png" width="100%">
</div>

<br>

---

## Delete Group

**`groupdel GROUP_NAME`**
**`groupdel --help`**

<div align="center">
  <img src="./assets/images/groupdel_help.png" width="100%">
</div>

<br>

**`groupdel group1`**

<div align="center">
  <img src="./assets/images/groupdel_group1.png" width="100%">
</div>

---

#### 2.4 Assign user to Primary and Secondary group

##### 2.4.1 Assign user to Primary Group

**`usermod -g GROUP_NAME USER_NAME`**

<div align="center">
  <img src="./assets/images/usermod_user1_primary_grp.png" width="100%">
</div>

<br>

##### 2.4.2 Assign user to Secondary Group

**`usermod -G GROUP_NAME USER_NAME`**

<div align="center">
  <img src="./assets/images/usermod_user1_secondary_grp.png" width="100%">
</div>

<br>

##### 2.4.3 Assign user to Multiple Secondaries Group

**`usermod -aG GROUP_NAME USER_NAME`**

<div align="center">
  <img src="./assets/images/usermod_user1_multiple_secondary_grp.png" width="100%">
</div>

---

#### 2.5 List all members in group

##### Package:`libuser`:_user and group account administration library - utilities_

**debian:`apt install libuser`**
**redhat:`yum install libuser.x86_64`**

<div align="center">
  <img src="./assets/images/list_users_in_group.png" width="100%">
</div>

---

#### 2.6 Remove members from group

<div align="center">
  <img src="./assets/images/remove_user_from_group.png" width="100%">
</div>

---

## [Outlines](../README.md)
