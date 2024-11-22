# Paddock Pal: Drive Through F1 Knowledge

### Authors
- Aniket Patole
- Saurabh Vyawahare
- Shreya Bage

## Introduction

**Paddock Pal** is an interactive, Retrieval-Augmented Generation (RAG) platform that aims to provide a comprehensive and engaging Formula 1 (F1) experience for fans, professionals, and even the governing bodies like the FIA. This platform offers easy access to a wealth of F1 information, including regulations, track details, driver profiles, and real-time data. Additionally, it seeks to mitigate controversial penalty decisions during races by providing FIA officials with regulation-based insights in real time. Paddock Pal will ultimately enhance fan engagement, transparency, and support data-driven decision-making for various stakeholders.

## Project Overview

### Scope
- **Paddock Pal** is designed as a web-based application that enhances the experience of F1 fans and professionals by integrating multiple sources of information and providing insights on regulations, race strategies, driver details, and more.
- **Data Sources** include publicly available datasets, real-time data from the OpenF1 API, and official regulation documents scraped from the FIA's website.
- **Technologies**: FastAPI for backend services, Pinecone for vector search, OpenAI GPT-4 for RAG-based queries, Streamlit for the user interface, and Scikit-Learn for a predictive game module.

### Features
- **Information Hub**: An educational resource providing details about drivers, tracks, and races.
- **Regulations RAG Bot**: A chatbot capable of answering complex regulation-based questions to assist fans, officials, and teams.
- **Real-Time Data API Chatbot**: Provides real-time standings and race-related queries using the OpenF1 API.
- **Predictive Game Module**: An interactive game that lets users predict race outcomes based on track, driver, and team selections.

### Stakeholders
- **Fans & FIA Officials**: Casual fans, avid F1 followers, and FIA officials looking for accurate, real-time regulation-based insights.
- **Teams & Drivers**: Access to regulation explanations, incident precedents, and predictive tools for race strategies.
- **Content Creators & Journalists**: A reliable source of data for articles, videos, and other content around F1.

## Problem Statement

### Current Challenges
- Access to **regulations** is complex, and there is no easy lookup for rules during incidents.
- **Data fragmentation** makes it cumbersome to compile historical data, regulatory documents, and race statistics.
- **Inconsistent penalties** can affect the credibility of the sport, creating frustration among fans and teams.

### Opportunities
- **Paddock Pal** can centralize regulations, historical data, and real-time updates, enhancing user understanding and engagement.
- The **RAG bot** provides the FIA with decision-making support during live incidents, increasing transparency and minimizing controversy.
- A **predictive game** can make engaging with F1 fun, increasing fan involvement and deepening their understanding of race dynamics.

## Methodology

### Data Sources
- **Official FIA Documents**: Scraped and stored in Amazon S3, with text extracted using Adobe Extractor.
- **OpenF1 API**: Real-time race standings, driver statistics, and historical results.
- **Custom Synthesized Data**: Examples of historical incidents and penalties for penalty prediction.

### Technologies and Tools
- **Backend**: FastAPI and Snowflake for data storage; Pinecone for vector search.
- **AI Processing**: OpenAI GPT-4 for natural language insights, Scikit-Learn for predictive modeling.
- **Frontend**: Streamlit to provide an interactive user interface.

### Data Pipeline Design
- **Data Ingestion**: Scraping FIA documents, extracting text, and gathering real-time data from OpenF1 API.
- **Data Storage**: Snowflake for structured data, Pinecone for vector embeddings, and Amazon S3 for unstructured content.
- **Data Processing**: Using OpenAI embeddings to generate RAG responses; predictive modeling with Scikit-Learn.

## Project Plan and Timeline

### Milestones and Deliverables
1. **Week 1**: Core Data Setup and Backend Foundation.
   - Set up data ingestion workflows, backend setup with FastAPI, and data storage in Snowflake and Pinecone.
2. **Week 2**: MVP Development.
   - Build primary features: Regulations RAG bot, Information Hub, and basic frontend.
3. **Week 3**: Predictive Game and Testing.
   - Develop predictive game, integrate it into the platform, and conduct testing.

## Resources and Team
- **Saurabh Vyawahare**: Backend development and FastAPI integration, API integration for real-time data.
- **Aniket Patole**: Pinecone integration, scraping FIA documents, storing data in S3 and Snowflake.
- **Shreya Bage**: Frontend development using Streamlit, focusing on creating a user-friendly and interactive experience.

## Risks and Mitigation Strategies
- **Time Constraint**: Focus on core features first, parallel development by the team.
- **Data Integration Challenges**: Standardize data formats, incrementally test integration.
- **API Reliability**: Backup historical data in Snowflake for offline capabilities.
- **Frontend & Backend Sync Issues**: Conduct regular sync tests and implement error logging.
- **Data Quality**: Manual verification of scraped data, use fallback responses for incomplete data.

## Expected Outcomes and Benefits
- **User Engagement**: Targeting 50 daily active users and a 30% retention rate within the first month.
- **Enhanced Knowledge**: Instant access to regulations and driver information.
- **Support for Decision-Making**: Help FIA officials, teams, and drivers make informed, transparent decisions.
- **Increased Engagement**: Interactive predictions to engage users with race dynamics and strategies.

## Conclusion

**Paddock Pal** aims to transform how F1 enthusiasts engage with the sport by centralizing information and providing easy access to critical insights. With regulation support for the FIA, a comprehensive information hub, and a predictive game module, Paddock Pal will improve fan interaction, ensure transparency, and support data-driven decisions during live races. The project is poised to make a significant impact on how Formula 1 is understood, enjoyed, and managed by various stakeholders, with scalability planned for future expansions into advanced analytics and other motorsports.

