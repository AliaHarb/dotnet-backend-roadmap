# 🗄️ Week 06 — SQL Database Design (ERD & Mapping)

## 🎯 Objective

Design a relational database schema for Musicana Records by identifying the required entities and defining the relationships between them.

## 📋 Requirements

Create a database design that includes the following entities:

1. **Musicians**
   - ID
   - Name
   - Address:
     - Street
     - City
   - Phone

2. **Instruments**
   - Unique Name
   - Musical Key

3. **Albums**
   - Unique Title
   - Copyright Date
   - Album Identifier

4. **Songs**
   - Unique Title
   - Author

## 🔗 Relationships

The database should support the following relationships:

1. **Musicians and Instruments**
   - A musician can play multiple instruments.
   - An instrument can be played by multiple musicians.

2. **Albums and Songs**
   - An album can contain multiple songs.
   - Each song belongs to one album.

3. **Musicians and Songs**
   - A musician can perform multiple songs.
   - A song can be performed by multiple musicians.

4. **Musicians and Albums**
   - Each album must have exactly one musician as its producer.
   - A musician can produce multiple albums.

## 💡 Expected Outcome

An ERD and relational database design for Musicana Records that represents all the required entities, attributes, and relationships.
