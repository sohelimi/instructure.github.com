## iOS and Android 2.0 Mobile App API Documentation

### General notes
In general, the Canvas mobile app APIs follow the same pattern as the online content in Canvas. Often, simply replacing the `http://` with `canvas-courses://` will take you to the relevant content inside the mobile apps

If the user is not currently signed into their mobile app, they'll be redirected to a login page for the given domain.

**iOS only**: If the user is already signed into a different domain than the one specified, an attempt will be made to load the content. If the user has the same email address registered with multiple school accounts, we can often still load the content correctly.

**Android only**: If the user is already signed into a different domain than the one specified, they'll be redirected to the activity stream and they'll receive a message letting them know they're already signed into a different domain. 


---
### Login
Log the user into the given domain, if not already logged in.

    canvas-courses://example.instructure.com     

---
### Announcements
Open the app to a list of announcements for a course: (**Android only**)

    canvas-courses://example.instructure.com/courses/:courseID/announcements/
    
Open the app to a specific announcement:

    canvas-courses://example.instructure.com/courses/:courseID/announcements/:announcementID

---
### Assignments
Open the app to a specific assignment

     canvas-courses://example.instructure.com/courses/:courseID/assignments/:assignmentID"    

---
### Conversations

Open the app to the Conversation inbox page page. (**Android only**)

    canvas-courses://example.instructure.com/conversations/      

Open the app to a specific conversation (**Android only**)

     canvas-courses://example.instructure.com/conversations/CONVERSATION_ID      

---
### Courses
Open the app to the list of the user's courses: (**Android only**)

    canvas-courses://example.instructure.com/courses/ 

Open the app to a specific course home page: (**Android only**)

    canvas-courses://example.instructure.com/courses/:courseID/


---
### Discussions

Open the app to a list of discussions for a course: (**Android only**)

    canvas-courses://example.instructure.com/courses/:courseID/discussion_topics/

Open the app to a specific discussion topic

     canvas-courses://example.instructure.com/courses/:courseID/discussion_topics/:topicID    
     canvas-courses://example.instructure.com/groups/:groupID/discussion_topics/:topicID    


---
### Files
Open the app to a specific file

     canvas-courses://example.instructure.com/files/:fileID    

---
### Grades
Open the app to the course grades page: (**Android only**)

    canvas-courses://example.instructure.com/courses/:courseID/grades/

---
### Pages
Open the app to the list of wiki pages: (**Android only**)

    canvas-courses://example.instructure.com/courses/:courseID/wiki/
    canvas-courses://example.instructure.com/courses/:courseID/pages/

Open the app to a specific wiki page:

     canvas-courses://example.instructure.com/courses/:courseID/pages/:pageName    
     canvas-courses://example.instructure.com/courses/:courseID/wiki/:pageName    
     canvas-courses://example.instructure.com/groups/:groupID/pages/:pageName    
     canvas-courses://example.instructure.com/groups/:groupID/wiki/:pageName    

---
### People
Open the app to the list of people in a course: (**Android only**)

    canvas-courses://example.instructure.com/courses/:courseID/people/
    canvas-courses://example.instructure.com/courses/:courseID/users/

---
### Quizzes
Open a specific quiz.

     canvas-courses://example.instructure.com/courses/:courseID/quizzes/:quizID    
