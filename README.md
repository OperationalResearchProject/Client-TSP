# ORA-Tsp-Client
This project is a TSP client connected to the  [Operational Research API](https://github.com/geoffreyp/OperationalResearchWebAPI)

## The travelling salesman problem
The travelling salesman problem (TSP) asks the following question: "Given a list of cities and the distances between each pair of cities, what is the shortest possible route that visits each city exactly once and returns to the origin city?"

[From Wikipedia, the free encyclopedia](https://en.wikipedia.org/wiki/Travelling_salesman_problem)

## How use the client ?
### Use hillclimber algorithm :
```
python Client.py -h
```

### Use tabou search algorithm : (in the next release of the [Operational Research API](https://github.com/geoffreyp/OperationalResearchWebAPI))
```
python Client.py -t
```


## Rebuild proto files
```
python -m grpc_tools.protoc -I=./proto --python_out=./protoGenerated --grpc_python_out=./protoGenerated proto/hcfi.proto
```
