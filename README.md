levenshtein
===========

[Go](http://golang.org) package to calculate the [Levenshtein Distance](http://en.wikipedia.org/wiki/Levenshtein_distance)

Install
-------

    go get github.com/arbovm/levenshtein

Example
-------

```go
package main

import (
	"fmt"
	"github.com/agnivade/levenshtein"
)

func main() {
	s1 := "kitten"
	s2 := "sitting"
	distance, err := levenshtein.ComputeDistance(s1, s2)
	if err != nil {
	  fmt.Errorf("Error returned- %s", err)
	}
	fmt.Printf("The distance between %s and %s is %d\n",
		s1, s2, distance) // -> The distance between kitten and sitting is 3
}

```

Documentation
-------------

Located [here](http://godoc.org/github.com/agnivade/levenshtein)
