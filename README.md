var sum = 0;
function arrSum(arr) {
	for (var i = 0; i < arr.length; i++) {
		if (typeof arr[i] === 'number') {
			sum += arr[i]; 
		} else {
			arrSum(arr[i]);
		}
	}
	return sum;
}
arrSum([1,2,[3,4],[4,[5]]]);
// answer = 19; elements = 4
