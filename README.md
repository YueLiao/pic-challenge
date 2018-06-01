### Examples of reading data:
**Assume that we want to get the annotation of a certain image** whose `imgname = 'indoor_02018.jpg'`, we can use `cv2` to read instance annotation: 

	ins = cv2.imread(imagename.replace('.jpg','.png'),cv2.IMREAD_GRAYSCALE)

the corresponding semantic segmentation annotation can be read likewise.

**To get the relation annotation whose annotation file name is 'relation.json', run:**

	rel = Relation()
	rel.loadAnnot('relation.json')

**To get the relation annotation of a certain image, for example, 'indoor_00002.jpg', run:**

	relation = rel.loadRelation('indoor_02018.jpg')




### Visualization
**To visualize the semantic segmentation map, we can run:**

	visualize_segmentation(segmentationMap, img)

**To visualize the instance map of a certain category, we can run:**

	visualize_instance(instanceMap, segmentationMap, oriImg)


**To visualize relation, run:**

	visualize_relation(relation, instanceMap, img)

`img` is the original image.

### Evaluation code is coming soon.


# pic-challenge
# pic-challenge
# pic-challenge
