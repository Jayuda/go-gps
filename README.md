# go-gps
simple golang gogpslocation (gps) calculations

```
package main

import(
    "https://github.com/Jayuda/go-gps"
    "fmt"
)

func main() {
     // Make a few points
     p := gogps.NewPoint(42.25, 120.2)
     p2 := gogps.NewPoint(30.25, 112.2)
     
     // find the great circle distance between them
     dist := p.GreatCircleDistance(p2)
     fmt.Printf("great circle distance: %d\n", dist)
}
```