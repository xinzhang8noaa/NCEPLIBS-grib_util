################################################################################
# This makefile was produced by fmjif at 17:21:11 on 97/02/24.
SHELL=  /bin/sh
CMD=    grbindex
FOPTS=  -g -O3 -assume noold_ldout_format -convert big_endian  -axCORE-AVX2
LOPTS=
INCS=
OBJS=   grbindex.o
#LIBS= -L/nwprod/lib -lw3nco_4 -lbacio_4
LIBS=   ${W3NCO_LIB4} ${BACIO_LIB4}
################################################################################
$(CMD): $(OBJS)
	ftn $(LOPTS) $(OBJS) $(LIBS) -o $(CMD)
$(OBJS):        makefile $(INCS)
grbindex.o:     grbindex.f
	ftn -c $(FOPTS) $*.f
clean:
	-rm -f $(OBJS)
