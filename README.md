# st10448871-summative-Cyberbot_Final
Cyberbot application with Full implementation with task manager, quiz, NLP simulation, and activity log

PROJECT OVERVIEW

The Cybersecurity Awareness Chatbot is a developed WPF-based desktop application designed to help educate South African citizens about cybersecurity threats. This application has:
•	Interactive chat interface with voice greeting
•	Cybersecurity education on passwords, scams, privacy, safe browsing, social engineering, malware, and 2FA
•	Task management system with MySQL database integration
•	Cybersecurity quiz with 12 questions and scoring
•	Natural Language Processing (NLP) simulation
•	Activity logging for tracking user actions

The application's purpose is:
To create an engaging, educational tool that helps users understand and protect themselves from cyber threats while also providing practical task management and knowledge testing features(Quiz).


GitHub Submission.
Github Repository link:
https://github.com/Benedict10448871/st10448871-summative-Cyberbot_Final.git
With 6 commits.

Video Presentation Link:
https://youtu.be/i0TNdBs1LiE


FEATURES IMPLEMENTED
Poe1
1. Voice Greeting - Plays greeting.wav at application startup
2. ASCII Art Display - Cybersecurity-themed logo in header
3. User Interaction - Personalized greetings using user's name
4. Keyword Recognition - Detects passwords, scams, privacy, phishing, browsing, social engineering, malware, 2FA
5. Input Validation - Handles empty input and unrecognized queries
POE2
6. Random Responses - Each topic has 3+ responses selected randomly
7. Conversation Flow - Handles follow-ups like "tell me more" and "another tip"
8. Memory and Recall - Stores the user name and the favorite cybersecurity topic
9. Sentiment Detection - Detects worried, curious, frustrated, positive, negative, neutral
POE3
10. Task Assistant - Add tasks with reminders stored in MySQL database
11. Cybersecurity Quiz - 12 questions with multiple choice and true/false
12. NLP Simulation - Intent detection with keyword matching
13. Activity Log - Tracks all user actions with timestamps

DATABASE STRUCTURE
Database Name: cybersecurity_chatbot
SQL Creation Script:
CREATE DATABASE cybersecurity_chatbot;
USE cybersecurity_chatbot;

CREATE TABLE tasks (
    id INT AUTO_INCREMENT PRIMARY KEY,
    user_name VARCHAR(100) NOT NULL,
    title VARCHAR(255) NOT NULL,
    description TEXT,
    reminder_date DATETIME,
    is_completed BOOLEAN DEFAULT FALSE,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
