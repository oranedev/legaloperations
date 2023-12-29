# Reunion360 Data Structure Overview 🌐

## 1. User Data Type 👤
Stores information about each user of the platform.

**Fields:**
- **Username/Email:** Text (for login identification) 📧
- **Password:** Password (encrypted for security) 🔒
- **FullName:** Text 📛
- **Role:** Text or Option set (e.g., Admin, Regular User, Guest) 🎭
- **ProfilePicture:** Image 🖼️
- **ContactInformation:** Text or structured data type (for phone number, address, etc.) 📞
- **RegisteredMeetings:** List of Meetings (to link users with their meetings) 📅
- **DocumentHistory:** List of Documents (to track documents associated with the user) 📚

## 2. Meeting Data Type 📆
Manages information related to virtual meetings.

**Fields:**
- **MeetingTitle:** Text 🏷️
- **MeetingDate:** Date 📅
- **MeetingTime:** Time ⏰
- **Organizer:** User (link to the User who organized the meeting) 👤
- **Participants:** List of Users 👥
- **Agenda:** Text or List of Texts 📋
- **MeetingNotes:** Text 📝
- **VotingResults:** List of Votes or Text (if applicable) 🗳️
- **AssociatedDocuments:** List of Documents 📄

## 3. Document Data Type 📁
Handles legal documents associated with meetings.

**Fields:**
- **DocumentTitle:** Text 🏷️
- **DocumentType:** Text or Option set (e.g., Contract, Report, Minutes) 📑
- **CreationDate:** Date 📅
- **LastModified:** Date 🔄
- **Owner:** User (link to the User who owns/created the document) 👤
- **RelatedMeeting:** Meeting (link to the associated meeting) 📆
- **DocumentFile:** File (for storing the actual document) 🗄️
- **Status:** Text or Option set (e.g., Draft, Final, Signed) 📊

## 4. Vote Data Type 🗳️
Included if the platform has voting functionality.

**Fields:**
- **Voter:** User (link to the User who voted) 👤
- **Meeting:** Meeting (link to the meeting where the vote occurred) 📆
- **VoteOption:** Text or Option set (e.g., Yes, No, Abstain) 📝
- **VoteTime:** Date and Time ⏰
