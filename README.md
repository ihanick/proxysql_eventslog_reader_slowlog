# `proxysql_eventslog_reader_slowlog`
The tool converts proxysql queries log to slow log format for further pt-query-digest check.
Forked from ProxySQL `tools/eventslog_reader_sample.cpp`.

## Usage:
```git clone https://github.com/ihanick/proxysql_eventslog_reader_slowlog.git
cd proxysql_eventslog_reader_slowlog
make
./eventslog_reader_slowlog /var/lib/proxysql/queries.log.00000001 | pt-query-digest | less -iS
```
