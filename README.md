# jdbc-notes

# What is jdbc
- JDBC stands for Java Database Connectivity which resides in java.sql package and contains Connection, Statement, PreparedStatement, CallableStatement, and ResultSet.

# Connection(I)
- Used to establish connection with database.

# PreparedStatement
- Use to execute parameterized sql query.
- Use this instead of Statement.

### Difference between executeQuery and executeUpdate
- **executeQuery**: used for retrieval queries.
- **executeUpdate**: used for deletion, update, and insert queries.

### PreparedStatement setter methods
- **setInt(int paramIndex, int value)**
- **setString(int paramIndex, String value)**
- and many more based on datatype you need to set.

# ResultSet
- Maintains a cursor pointing to a row of a table. By default it points at 0 hence the indexing starts at 1.

### ResultSet indexing methods
- **next**: move to next row.
- **previous**: move back from previous row.
- **first**: move to first row of the result set.
- **last**: move to last row of the result set.

### ResultSet fetching methods
- **getInt(int columnIndex)**
- **getInt(String columnName)**

