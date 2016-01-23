FILES :=              \
    Hello             \
    UnitTests1        \
    UnitTests2        \
    UnitTesst3        \
    Coverage1         \
    Coverage2         \
    Coverage3

%.pyx: %.py
	./$<

%.pyy: %.py
	coverage run --branch ./$<
	coverage report -m

clean:
	rm -f  .coverage
	rm -f  *.pyc
	rm -rf __pycache__

testx: $(FILES:=.pyx)

testy: $(FILES:=.pyy)
