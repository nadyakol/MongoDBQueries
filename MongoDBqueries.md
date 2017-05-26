1. `db.test.find({ scores : {$elemMatch: {score:{$gt: 87, $lt:93}}} });`
1. `db.test.aggregate([{$unwind: "$scores"}, {$match: {"scores.type": "exam", "scores.score":{$gt: 90}}}]);`
1. `db.test.update({"name": "Dusti Lemmond"}, {$set: {"accepted": true}}, {multi: true});`
