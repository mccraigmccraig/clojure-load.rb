= clojure-load.rb

== DESCRIPTION:

a loader for clojure. configures java classpath with minimal fuss

== FEATURES:

- configure java classpath and exec clojure
- single arg inclusion of clojure projects with standard layout
- single arg inclusion of dirs of jars
- single arg inclusion of individual jars and dirs
- pass arbitrary jvm options
- pass arbitrary clojure script args
- clojure repos with standard layout can be included with a single arg

== PROBLEMS:

== SYNOPSIS:

# invoke clojure.lang.Script with both java and script args
/path/to/clojure-load.rb/clojure -l clojure-contrib -- -Xmx1g -- script args

# invoke clojure.lang.Script with script args
/path/to/clojure-load.rb/clojure -l clojure-contrib -l incanter -- script args

# invoke clojure.lang.Repl with java args only
/path/to/clojure-load.rb/clojure -l clojure-contrib -l incanter -- -Xmx1g --

== REQUIREMENTS:

- java
- clojure git repo [ in same dir as clojure-load.rb repo for default operation ]
- other clojure repos in same dir, for single arg includes

== INSTALL:

git clone git://github.com/mccraigmccraig/clojure-load.rb.git

== LICENSE:

(The BSD License)

Copyright (c) 2009, craig mcmillan
All rights reserved.

Redistribution and use in source and binary forms, with or without modification,
are permitted provided that the following conditions are met:

  * Redistributions of source code must retain the above copyright notice,
    this list of conditions and the following disclaimer.
  * Redistributions in binary form must reproduce the above copyright notice,
    this list of conditions and the following disclaimer in the documentation
    and/or other materials provided with the distribution.
  * Neither the name of the <ORGANIZATION> nor the names of its contributors may
    be used to endorse or promote products derived from this software without
    specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
