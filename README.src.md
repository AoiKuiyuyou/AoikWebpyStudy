[:var_set('', """
# Compile command
aoikdyndocdsl -s README.src.md -n aoikdyndocdsl.ext.all::nto -g README.md
""")
]\
[:HDLR('heading', 'heading')]\
# AoikWebpyStudy
Python **web.py** library study.

Tested working with:
- Python 2.7
- web.py 0.38

Trace call using [AoikTraceCall](https://github.com/AoiKuiyuyou/AoikTraceCall):
- [RequestHandlerWSGIServerTraceCall.py](/src/RequestHandlerWSGIServerTraceCall.py)
- [RequestHandlerWSGIServerTraceCallLogPy2.txt](/src/RequestHandlerWSGIServerTraceCallLogPy2.txt?raw=True)
- [RequestHandlerWSGIServerTraceCallNotesPy2.txt](/src/RequestHandlerWSGIServerTraceCallNotesPy2.txt?raw=True)

## Table of Contents
[:toc(beg='next', indent=-1)]

## Set up AoikTraceCall
[:tod()]

### Setup via pip
Run:
```
pip install git+https://github.com/AoiKuiyuyou/AoikTraceCall
```

### Setup via git
Run:
```
git clone https://github.com/AoiKuiyuyou/AoikTraceCall

cd AoikTraceCall

python setup.py install
```

## Usage
[:tod()]

### Start server
Run:
```
python "AoikWebpyStudy/src/RequestHandlerWSGIServerTraceCall.py" > Log.txt 2>&1
```

### Send request
Run:
```
curl -X POST -d hello http://127.0.0.1:8000/
```
