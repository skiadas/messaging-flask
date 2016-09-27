# Initial specifications

This document describes the broad goals of the application.

- There is no elaborate user system. Users are simply recognized by their "logins". Logins cannot exceed 20 characters.
- Users can send "messages" to each other. A message simply has a sender, a recipient, a subject line that cannot exceed 140 characters, and a text body that cannot exceed 500 characters.
    - It should be an error if a message has an empty recipient or sender name. But the sender/recipient don't need to pre-exist in the system.
    - Messages get a timestamp for when they were submitted.
    - Messages get a mark on whether they have been "read" or not. All messages start as unread.
    - Messages have a "priority" level, which must be "Low", "Normal", or "High". This is set when the message is sent, and cannot be changed.
- A user should be able to see all the messages they have sent, along with their "read" status.
- A user should be able to see all the messages they have received. They should be able to mark messages as read. They should not be able to undo that action.
- Both message lists should be sortable and filterable in various ways.