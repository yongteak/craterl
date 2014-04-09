crate-erlang
============

Erlang client for crate.

Installation
------------

```
rebar get-deps
rebar compile
```

Shell
-----

Get all the stuff on an erlang shell:

```
erl -pa ebin deps/*/ebin
```

Use library from erlang shell, for testing, debuggin etc.:

```
1> crate_erlang:start().
ok
5> crate_erlang:sql(<<"insert into table stuff (id, name) values (?, ?)">>, [1, <<"craty">>]).
...
```

Tests
-----

Simply call ```rebar eunit skip_deps=true``` to run the tests for crate_erlang.


