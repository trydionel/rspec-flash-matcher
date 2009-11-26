RSpec Flash Matcher
===================

What It Does
------------

This is a simple RSpec matcher to help with testing the Rails flash.
Instead of
`it "should set the error flash" do
	flash[:error].should_not be_nil
end`
just use
`it { should set_flash(:error) }`

If you like testing for exact output, you can use
`it { should set_flash(:error).to("OMG u broked it") }`

TODO
----

- Add support for regex matching
