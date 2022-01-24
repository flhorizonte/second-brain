### For In and For Of

	```javascript
			let list = [4, 5, 6];
			
			for (let i in list) {
			   console.log(i); // "0", "1", "2",
			}
			
			for (let i of list) {
			   console.log(i); // "4", "5", "6"
			}
	```

- For In - Itera o array sobre seus indices.
- For Of - Itera o array sobre seus valores.