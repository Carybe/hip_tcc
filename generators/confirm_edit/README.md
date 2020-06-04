# ENV
## Using Virtualenv:
```bash
	mkdir env
	virtualenv -p python2 env
	. env/bin/activate
	pip install -r src/requirements.txt
```
## Using Conda:
```bash
	conda create -n wikimedia python=2.7 pillow
	conda activate wikimedia
```
# RUN
```bash
	python captcha.py          \
		--random           \
		--key 'teste'      \
		--output out       \
		--min-length 6     \
		--max-length 6     \
		--threads $(nproc) \
		--count 2000       \
		--font /usr/share/fonts/truetype/liberation/LiberationMono-Regular.ttf
```

# DOC
See output of `python captcha.py --help`
