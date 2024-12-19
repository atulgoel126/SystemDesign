# Notification System for Blogging Website

## Context
I recently had an interview with a company, where I was asked this question about System Design. It didn't go great, and I realized I need to practice giving interviews.
The chief problem was communication - I found it hard to convert my thoughts into coherent sentences. 
I was speaking ALL of my thoughts aloud, which only added to the interviewer's confusion.

From the interviewer's side, he gave me ample hints but the conversation didn't go as well as either of us had hoped for.

This is my second attempt at the same System Design problem to understand how I could have done better.


## Problem Statement

We have to design a website like Medium with emphasis on posting an article.

In the second part, we need to augment this system to handle notifications.
Users can subscribe to authors such that whenever an author posts, all the subscribers should get an notification.
For simplicity, we'll only consider an email notification.


### Requirements

The first step was to gather the requirements for the first half. Based on our conversation, they were:

- Ability to publish a blog post
- View it publicly
- ~~Edit only by author~~
- ~~View only after publish~~
- ~~Ability to save it as a draft~~

For simplicity, we'll consider the simple model of making a post and saving it in the database. 

The second part had these requirements:

- Sending email notifications to all subscribers
    - This isn't realtime, the process can take a while
    - Every subscriber must get an email for every post
    - The system needs to be resilient to failures. If a system breaks in between sending a large of emails, it should continue from where it left.

---

## Solution

### Overview


### High Level Design
```mermaid

```

### Low Level Design

### Choice of Database


### Caching
Avoid this for now


### Database Design

---

## Request Processing Flow

### 1. Happy Path - making a post

- **Steps**:
- **Outcome**: The request is processed immediately and successfully.

### 2. Happy Path - sending notifications to subscribers

- **Steps**:
- **Outcome**: An email is sent to all the subscribers

### 3. Some error occurred while sending notifications

- **Steps**:
  - 
- **Outcome**: The notification is delayed but eventually sent to all subscribers

### 3. Processing Fails for a Request

---

## Follow ups


### **1. Question?**
Answer

## Areas for improvement

### 1. Use X instead of Y