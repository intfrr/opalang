### if Opa has been compiled with Dbm support, nothing to add
### (uncomment if Opa compiler is without Dbm support)
# # dbm is in a subdirectory of ocaml libs
# INCLUDE=-I +dbm
# LINK=dbm.cmxa


all : plugin opa

plugin:
	$(OPA_PLUGIN_BUILDER) $(INCLUDE) -o dbm dbm.ml

opa:
	$(OPA) $(INCLUDE) $(LINK) dbm.opp dbm.opa

clean:
	rm -rf _build _tracks dbm.opp dbm.exe *.log
