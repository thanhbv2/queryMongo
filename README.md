# queryMongo

```js
// 
db.attendances.aggregate([
	{$match: {type: "Holiday"}},
	{$project: 
		{count: {$size: "$works"}}
	
	},
	{$match: {count: {$gt: 1}}}

])

```
