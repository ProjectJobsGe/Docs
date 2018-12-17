# ProjectJobsGe API - კონტრაქტი

```Date formats used in this document are ISO 8601 comliant, see more at: https://www.w3.org/TR/NOTE-datetime```

## GET `/jobs`
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
      "jobsGeID": "200018",
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
      "jobsGeID": "199995"
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

## GET `/job`
Single job endpoint

```JSON
{
  "data": {
    "type": "job",
    "id": "1",
    "attributes": {
      "jobsGeID": "200018",
      "title": "წარმოების ინჟინერ-კონსტრუქტორი",
      "publicationDate": "1997-07-16T19:20:30+01:00",
      "expirationDate":  "1997-08-16T19:20:30+01:00", 
      "organization": "The Stream",
      "adType": "ვაკანსია",
      "location": "თბილისი",
      "category": "ტექნიკური/ლოჯისტიკა",
      "text": "განცახდების სრული ტექსტი"
    }
  },
  "links": {
    "self": "http://example.com/jobs/1"
  }
}
```


## POST `/jobs`
Creating jobs resources.

```JSON
{
  "data": [{
      "type": "job",
      "id": "1",
      "attributes": {
        "jobsGeID": "200018",
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
        "jobsGeID": "199995"
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


