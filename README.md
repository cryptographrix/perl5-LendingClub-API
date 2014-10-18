LendingClub-API
===============

This module is the start of a LendingClub API perl5 module.

So far, anything that requires a GET has been implemented.

SYNOPSIS
--------

    use LendingClub::API;
    use Data::Dumper;

    # public functions do not require any options
    my $lcapi_object = new LendingClub::API( "this-is-not-a-real-investor-id", "this-is-not-a-real-key" );

    print Dumper( $lcapi_object->available_cash() ) ."\n";
    print Dumper( $lcapi_object->summary() ) ."\n";

    print Dumper( $lcapi_object->notes_owned() ) ."\n";
    print Dumper( $lcapi_object->detailed_notes_owned() ) ."\n";

    print Dumper( $lcapi_object->portfolios_owned() ) ."\n";
    print Dumper( $lcapi_object->listed_loans() ) ."\n";


TODO
----

- Anything that requires a POST.

- Basic error handling based on the documentation at https://www.lendingclub.com/developers/lc-api.action


INSTALLATION
------------

To install this module, run the following commands:

	perl Makefile.PL
	make
	make test
	make install


LICENSE
-------
Beerware license
