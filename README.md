# booblesort

```go
func main() {
	nums := []int{7, 4, 5, 3, 1, 2, 6, 0}
	count := len(nums)
	counter := 0
	for counter >= 0 {
		for i := 0; i < count-1; i++ {
			if nums[i] > nums[i+1] {
				nums[i+1], nums[i] = nums[i], nums[i+1]
				counter++
			}
		}
		counter--
	}
	fmt.Println(nums)
}
```
