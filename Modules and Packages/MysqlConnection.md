``c
import mysql.connector

# Connect to MySQL database
conn = mysql.connector.connect(
    host="localhost",        # MySQL server address
    user="root",    # Your MySQL username
    password="mgpatils",# Your MySQL password
    database="patils" # The database you want to use
)

cursor = conn.cursor()

# Create a table (if it doesn't already exist) without the age column
cursor.execute('''
    CREATE TABLE IF NOT EXISTS users (
        id INT AUTO_INCREMENT PRIMARY KEY,
        name VARCHAR(100)
    )
''')

# Insert more data into the table (without age)
cursor.execute("INSERT INTO users (name) VALUES (%s)", ('Alice',))
cursor.execute("INSERT INTO users (name) VALUES (%s)", ('Bob',))
cursor.execute("INSERT INTO users (name) VALUES (%s)", ('Charlie',))
cursor.execute("INSERT INTO users (name) VALUES (%s)", ('David',))
cursor.execute("INSERT INTO users (name) VALUES (%s)", ('Eve',))
cursor.execute("INSERT INTO users (name) VALUES (%s)", ('Frank',))

# Commit the transaction
conn.commit()

# Query the data
cursor.execute("SELECT * FROM users")

# Fetch all the results
rows = cursor.fetchall()

# Display the results
for row in rows:
    print(f"ID: {row[0]}, Name: {row[1]}")

# Close the connection
cursor.close()
conn.close()
``
