.. The contents of this file may be included in multiple topics (using the includes directive).
.. The contents of this file should be modified in a way that preserves its ability to appear in multiple topics.

.. To test if a file is a block device:

.. code-block:: ruby

   describe file('/dev/zero') do
     its('type') { should eq 'block' }
     it { should be_character_device }
     it { should_not be_file }
     it { should_not be_directory }
   end
