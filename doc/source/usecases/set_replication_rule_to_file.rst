..
      Copyright European Organization for Nuclear Research (CERN)

      Licensed under the Apache License, Version 2.0 (the "License");
      You may not use this file except in compliance with the License.
      You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0

------------------------------------------
Set a replication rule on an existing file
------------------------------------------

.. sequence-diagram::

   client:PythonClient
   core:rucioserver "RucioCore"

   client:core[s].setreplicationRules(**)
   core[s]:core.registerTransfers(**)
