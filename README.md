# saytifical
say it scientifically

# How to
- Start server/db: mongod --dbpath data/
    - open http://localhost:27017/
- If the server is already running:
    - ps wuax | grep mongo
    - sudo kill <PID>
- Delete db: mongo <dbname> --eval "db.dropDatabase()"
- Create db (e.g., saytifical):
    - mongo
    - use saytifical
    - db.saytifica.insert([{
          "name" : "Priming effect",
          "definition" : "Priming is an implicit memory effect in which exposure to one stimulus influences a response to another stimulus.",
          "aka" : "Context priming",
          "video" : "HRAKt0GakJM",
          "category" : "Psychology",
          "icon" : "priming_effect.jpg"
        }])
    - db.saytifica.find().pretty()
- npm install && npm start
    - http://localhost:3000/saytifica
