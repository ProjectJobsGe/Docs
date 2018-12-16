# ProjectJobsGe API - კონტრაქტი

```Date formats used in this document are ISO 8601 comliant, see more at: https://www.w3.org/TR/NOTE-datetime```

## `/jobs`
Jobs listing endpoint

```JSON
{
  "links": {
    "self": "http://example.com/jobs"
  },
  "data": [{
    "type": "job",
    "id": "1",
    "attributes": {
      "title": "წარმოების ინჟინერ-კონსტრუქტორი",
      "publicationDate": "1997-07-16T19:20:30+01:00",
      "expirationDate":  "1997-08-16T19:20:30+01:00", 
      "organization": "The Stream",
      "adType": "ვაკანსია",
      "location": "თბილისი",
      "category": "ტექნიკური/ლოჯისტიკა",
      "text": "განცახდების სრული ტექსტი"
    }
  }, {
    "type": "job",
    "id": "2",
    "attributes": {
      "title": "Front-End დეველოპერი",
      "publicationDate": "2003-03-14T11:10:10+01:00",
      "expirationDate":  "2003-04-14T11:10:10+01:00",
      "organization": "კრედო ბანკი",
      "adType": "ტრენინგი",
      "location": "ქუთაისი",
      "category": "საინფორმაციო ტექნოლოგიები",
      "text": "განცახდების სრული ტექსტი"
    }
  }]
}
```
