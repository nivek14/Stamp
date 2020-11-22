BayesVar32:
	for t in 2 4 8 16 32 64 ; do \
        #n=1 ; while [ $${n} -le 5 ] ; do \
		for n in $$(seq 1 30) ; do \
			OMP_NUM_THREADS=$$t ./bayes -v32 -r4096 -n10 -p40 -i2 -e8 -s1 -t $$t >> bayesVar32Out$$t.txt ; \
        done ; \
    done ;

	#gnuplot outerboxplot.gnu

BayesVar64:
	for t in 2 4 8 16 32 64 ; do \
        #n=1 ; while [ $${n} -le 5 ] ; do \
		for n in $$(seq 1 30) ; do \
			OMP_NUM_THREADS=$$t ./bayes -v64 -r4096 -n10 -p40 -i2 -e8 -s1 -t $$t >> bayesVar64Out$$t.txt ; \
        done ; \
    done ;

	#gnuplot outerboxplot.gnu
	
BayesVar128:
	for t in 2 4 8 16 32 64 ; do \
        #n=1 ; while [ $${n} -le 5 ] ; do \
		for n in $$(seq 1 30) ; do \
			OMP_NUM_THREADS=$$t ./bayes -v128 -r4096 -n10 -p40 -i2 -e8 -s1 -t $$t >> bayesVar128Out$$t.txt ; \
        done ; \
    done ;

	#gnuplot outerboxplot.gnu
