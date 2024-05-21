# Comparing `tmp/tmticket-0.2.15.tar.gz` & `tmp/tmticket-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmticket-0.2.15.tar", last modified: Tue May 21 01:49:42 2024, max compression
+gzip compressed data, was "tmticket-0.2.2.tar", last modified: Wed May  8 00:06:29 2024, max compression
```

## Comparing `tmticket-0.2.15.tar` & `tmticket-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 01:49:42.037801 tmticket-0.2.15/
--rw-r--r--   0 root         (0) root         (0)      279 2024-05-21 01:49:42.037801 tmticket-0.2.15/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 01:49:42.034801 tmticket-0.2.15/pytmtickets/
--rw-r--r--   0 root         (0) root         (0)      363 2024-05-21 01:47:21.000000 tmticket-0.2.15/pytmtickets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3178 2024-05-21 01:46:27.000000 tmticket-0.2.15/pytmtickets/client.py
--rw-r--r--   0 root         (0) root         (0)    12664 2024-05-21 01:46:46.000000 tmticket-0.2.15/pytmtickets/model.py
--rw-r--r--   0 root         (0) root         (0)     4734 2024-05-21 01:47:10.000000 tmticket-0.2.15/pytmtickets/query.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 01:49:42.037801 tmticket-0.2.15/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      522 2024-05-21 01:48:57.000000 tmticket-0.2.15/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 01:49:42.036801 tmticket-0.2.15/tmticket.egg-info/
--rw-r--r--   0 root         (0) root         (0)      279 2024-05-21 01:49:41.000000 tmticket-0.2.15/tmticket.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      255 2024-05-21 01:49:41.000000 tmticket-0.2.15/tmticket.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 01:49:41.000000 tmticket-0.2.15/tmticket.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-21 01:49:41.000000 tmticket-0.2.15/tmticket.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-05-21 01:49:41.000000 tmticket-0.2.15/tmticket.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:06:29.254469 tmticket-0.2.2/
+-rw-r--r--   0 root         (0) root         (0)     1067 2024-05-07 22:01:04.000000 tmticket-0.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      736 2024-05-08 00:06:29.253469 tmticket-0.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-07 22:01:04.000000 tmticket-0.2.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-08 00:06:29.254469 tmticket-0.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      968 2024-05-08 00:06:04.000000 tmticket-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:06:29.250469 tmticket-0.2.2/tmticket/
+-rw-r--r--   0 root         (0) root         (0)      363 2024-05-08 00:06:04.000000 tmticket-0.2.2/tmticket/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5702 2024-05-08 00:06:04.000000 tmticket-0.2.2/tmticket/client.py
+-rw-r--r--   0 root         (0) root         (0)    13241 2024-05-08 00:06:04.000000 tmticket-0.2.2/tmticket/model.py
+-rw-r--r--   0 root         (0) root         (0)     4525 2024-05-08 00:06:04.000000 tmticket-0.2.2/tmticket/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:06:29.252469 tmticket-0.2.2/tmticket.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      736 2024-05-08 00:06:28.000000 tmticket-0.2.2/tmticket.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      261 2024-05-08 00:06:29.000000 tmticket-0.2.2/tmticket.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 00:06:28.000000 tmticket-0.2.2/tmticket.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-08 00:06:28.000000 tmticket-0.2.2/tmticket.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-08 00:06:28.000000 tmticket-0.2.2/tmticket.egg-info/top_level.txt
```

### Comparing `tmticket-0.2.15/pytmtickets/model.py` & `tmticket-0.2.2/tmticket/model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,356 +1,360 @@
-import aiohttp
+"""Models for API objects"""
+from datetime import datetime
 import re
+import aiohttp  # Assuming aiohttp is used for async operations
 
 def _assign_links(obj, json_obj, base_url=None):
     """Assigns `links` attribute to an object from JSON"""
-    json_links = json_obj.get('_links', {})
-    obj_links = {}
-    for k, v in json_links.items():
-        if 'href' in v:
-            href = re.sub(r"\{.+?\}", "", v['href'])
-            if base_url:
-                href = f"{base_url}{href}"
-            obj_links[k] = href
-        else:
-            obj_links[k] = v
-    obj.links = obj_links
+    json_links = json_obj.get('_links')
+    if not json_links:
+        obj.links = {}
+    else:
+        obj_links = {}
+        for k, v in json_links.items():
+            if 'href' in v:
+                href = re.sub("({.+})", "", v['href'])
+                if base_url:
+                    href = f"{base_url}{href}"
+                obj_links[k] = href
+            else:
+                obj_links[k] = v
+        obj.links = obj_links
 
-class Page:
+class Page(list):
     """API response page"""
-    def __init__(self, items=None, links=None, number=None, size=None, total_elements=None, total_pages=None):
-        self.items = items or []
-        self.links = links or {}
+    def __init__(self, number=None, size=None, total_elements=None, total_pages=None):
+        super().__init__([])
         self.number = number
         self.size = size
         self.total_elements = total_elements
         self.total_pages = total_pages
 
     @staticmethod
     def from_json(json_obj):
-        """Instantiate and return a Page object from JSON"""
-        items = json_obj.get('_embedded', {}).get('events', [])
-        links = json_obj.get('_links', {})
-        page_data = json_obj.get('page', {})
-        return Page(
-            items=items,
-            links=links,
-            number=page_data.get('number', 0),
-            size=page_data.get('size', 0),
-            total_elements=page_data.get('totalElements', 0),
-            total_pages=page_data.get('totalPages', 0)
-        )
-
-    def __iter__(self):
-        return iter(self.items)
+        """Instantiate and return a Page(list)"""
+        pg = Page()
+        pg.number = json_obj['page']['number']
+        pg.size = json_obj['page']['size']
+        pg.total_pages = json_obj['page']['totalPages']
+        pg.total_elements = json_obj['page']['totalElements']
+        _assign_links(pg, json_obj)
+        # Assuming implementation for adding items to the page based on 'events', 'venues', etc.
+        return pg
 
 class Event:
     """Ticketmaster event"""
     def __init__(self, event_id=None, name=None, start_date=None, start_time=None, status=None, classifications=None, links=None):
         self.id = event_id
         self.name = name
         self.start_date = start_date
         self.start_time = start_time
         self.status = status
-        self.classifications = classifications or []
-        self.links = links or {}
+        self.classifications = classifications
+        self.links = links
 
     @staticmethod
     def from_json(json_event):
         """Creates an `Event` from API's JSON response"""
-        event = Event(
-            event_id=json_event.get('id'),
-            name=json_event.get('name'),
-            start_date=json_event.get('dates', {}).get('start', {}).get('localDate'),
-            start_time=json_event.get('dates', {}).get('start', {}).get('localTime'),
-            status=json_event.get('dates', {}).get('status', {}).get('code'),
-            classifications=[Classification.from_json(cl) for cl in json_event.get('classifications', [])]
-        )
-        _assign_links(event, json_event)
-        return event
-
-    def to_dict(self):
-        """Convert the Event object to a dictionary for serialization"""
-        return {
-            'id': self.id,
-            'name': self.name,
-            'start_date': self.start_date,
-            'start_time': self.start_time,
-            'status': self.status,
-            'classifications': [cl.to_dict() for cl in self.classifications],
-            'links': self.links,
-        }
+        e = Event()
+        e.id = json_event.get('id')
+        e.name = json_event.get('name')
+        # Additional attributes setup
+        _assign_links(e, json_event)
+        return e
 
     async def fetch_additional_details(self):
         """Asynchronously fetch additional event details (hypothetical example)"""
         async with aiohttp.ClientSession() as session:
             async with session.get(self.links['self']) as response:
                 details = await response.json()
                 # Process and update event instance with additional details
 
 class Venue:
     """A Ticketmaster venue."""
-    def __init__(self, name=None, address=None, city=None, state_code=None, postal_code=None, latitude=None, longitude=None, timezone=None, links=None, **kwargs):
+    def __init__(self, name=None, address=None, city=None, state_code=None,
+                 postal_code=None, latitude=None, longitude=None,
+                 markets=None, url=None, box_office_info=None,
+                 dmas=None, general_info=None, venue_id=None,
+                 social=None, timezone=None, images=None,
+                 parking_detail=None, accessible_seating_detail=None,
+                 links=None):
         self.name = name
+        self.id = venue_id
         self.address = address
+        self.postal_code = postal_code
         self.city = city
         self.state_code = state_code
-        self.postal_code = postal_code
         self.latitude = latitude
         self.longitude = longitude
         self.timezone = timezone
-        self.links = links or {}
-        for key, value in kwargs.items():
-            setattr(self, key, value)
-
-    @staticmethod
-    def from_json(json_venue):
-        """Returns a `Venue` object from JSON"""
-        venue = Venue(
-            name=json_venue.get('name'),
-            address=json_venue.get('address', {}).get('line1'),
-            city=json_venue.get('city', {}).get('name'),
-            state_code=json_venue.get('state', {}).get('stateCode'),
-            postal_code=json_venue.get('postalCode'),
-            latitude=json_venue.get('location', {}).get('latitude'),
-            longitude=json_venue.get('location', {}).get('longitude'),
-            timezone=json_venue.get('timezone'),
-        )
-        _assign_links(venue, json_venue)
-        return venue
-
-    def to_dict(self):
-        """Convert the Venue object to a dictionary for serialization"""
+        self.url = url
+        self.box_office_info = box_office_info
+        self.dmas = dmas
+        self.markets = markets
+        self.general_info = general_info
+        self.social = social
+        self.images = images
+        self.parking_detail = parking_detail
+        self.accessible_seating_detail = accessible_seating_detail
+        self.links = links
+
+    @property
+    def location(self):
+        """Location-based data (full address, lat/lon, timezone)"""
         return {
-            'name': self.name,
             'address': self.address,
+            'postal_code': self.postal_code,
             'city': self.city,
             'state_code': self.state_code,
-            'postal_code': self.postal_code,
-            'latitude': self.latitude,
-            'longitude': self.longitude,
             'timezone': self.timezone,
-            'links': self.links,
+            'latitude': self.latitude,
+            'longitude': self.longitude
         }
 
+    @staticmethod
+    def from_json(json_venue):
+        """Returns a `Venue` object from JSON"""
+        v = Venue()
+        v.id = json_venue.get('id')
+        v.name = json_venue.get('name')
+        v.url = json_venue.get('url')
+        v.postal_code = json_venue.get('postalCode')
+        v.timezone = json_venue.get('timezone')
+        v.address = json_venue['address'].get('line1')
+        v.city = json_venue['city'].get('name')
+        v.state_code = json_venue['state'].get('stateCode')
+        v.latitude = json_venue['location'].get('latitude')
+        v.longitude = json_venue['location'].get('longitude')
+        # Process additional attributes as before
+        _assign_links(v, json_venue)
+        return v
+
     async def fetch_additional_details(self, api_client):
-        """Asynchronously fetch additional venue details."""
-        details_url = self.links.get('self')
+        """Asynchronously fetch additional venue details.
+        
+        Args:
+            api_client: Instance of an asynchronous API client.
+        """
+        # Example URL construction, adjust based on your API's design
+        details_url = self.links.get('self', '')  # Assuming 'self' link is detailed info
         if details_url:
-            additional_details = await api_client.get_url(details_url)
+            additional_details = await api_client.get(details_url)
             # Process and integrate additional_details into the Venue instance
+            print(additional_details)  # Placeholder for actual processing logic
 
     def __str__(self):
-        return f"{self.name} at {self.address} in {self.city}, {self.state_code}"
+        return f"{self.name} at {self.address} in {self.city} {self.state_code}"
 
 class Attraction:
     """Attraction"""
-    def __init__(self, attraction_id=None, attraction_name=None, url=None, classifications=None, images=None, test=None, links=None):
+    def __init__(self, attraction_id=None, attraction_name=None, url=None,
+                 classifications=None, images=None, test=None, links=None):
         self.id = attraction_id
         self.name = attraction_name
         self.url = url
-        self.classifications = classifications or []
-        self.images = images or []
+        self.classifications = classifications
+        self.images = images
         self.test = test
-        self.links = links or {}
+        self.links = links
 
     @staticmethod
     def from_json(json_obj):
         """Convert JSON object to `Attraction` object"""
-        att = Attraction(
-            attraction_id=json_obj.get('id'),
-            attraction_name=json_obj.get('name'),
-            url=json_obj.get('url'),
-            test=json_obj.get('test', False),
-            images=json_obj.get('images', []),
-            classifications=[Classification.from_json(cl) for cl in json_obj.get('classifications', [])]
-        )
+        att = Attraction()
+        att.id = json_obj.get('id')
+        att.name = json_obj.get('name')
+        att.url = json_obj.get('url')
+        att.test = json_obj.get('test', False)  # Assuming 'test' is a boolean field
+        att.images = json_obj.get('images', [])
+        classifications = json_obj.get('classifications', [])
+        att.classifications = [Classification.from_json(cl) for cl in classifications]
         _assign_links(att, json_obj)
         return att
 
-    def to_dict(self):
-        """Convert the Attraction object to a dictionary for serialization"""
-        return {
-            'id': self.id,
-            'name': self.name,
-            'url': self.url,
-            'classifications': [cl.to_dict() for cl in self.classifications],
-            'images': self.images,
-            'test': self.test,
-            'links': self.links,
-        }
-
     async def fetch_additional_details(self, api_client):
-        """Asynchronously fetch additional details for the attraction."""
-        details_url = self.links.get('self')
+        """Asynchronously fetch additional details for the attraction.
+        
+        Args:
+            api_client: Instance of an asynchronous API client capable of making GET requests.
+        """
+        details_url = self.links.get('self', '')  # Example, adjust based on actual API design
         if details_url:
-            additional_details = await api_client.get_url(details_url)
-            # Process and integrate additional_details into the Attraction instance
+            async with api_client.session.get(details_url) as response:
+                details_json = await response.json()
+                # Here you would process the details_json to extract and integrate additional details
+                print(details_json)  # Placeholder for actual logic
 
     def __str__(self):
         return self.name if self.name is not None else 'Unknown'
 
+
 class Classification:
     """Classification object (segment/genre/sub-genre)"""
     def __init__(self, segment=None, classification_type=None, subtype=None, primary=None, links=None):
         self.segment = segment
         self.type = classification_type
         self.subtype = subtype
         self.primary = primary
-        self.links = links or {}
+        self.links = links
 
     @staticmethod
     def from_json(json_obj):
-        cl = Classification(
-            primary=json_obj.get('primary'),
-            segment=Segment.from_json(json_obj['segment']) if 'segment' in json_obj else None,
-            classification_type=ClassificationType.from_json(json_obj['type']) if 'type' in json_obj else None,
-            subtype=ClassificationSubType.from_json(json_obj['subType']) if 'subType' in json_obj else None
-        )
+        cl = Classification()
+        cl.primary = json_obj.get('primary')
+
+        if 'segment' in json_obj:
+            cl.segment = Segment.from_json(json_obj['segment'])
+
+        if 'type' in json_obj:
+            cl.type = ClassificationType(json_obj['type']['id'], json_obj['type']['name'])
+
+        if 'subType' in json_obj:
+            cl.subtype = ClassificationSubType(json_obj['subType']['id'], json_obj['subType']['name'])
+
         _assign_links(cl, json_obj)
         return cl
 
-    def to_dict(self):
-        """Convert the Classification object to a dictionary for serialization"""
-        return {
-            'segment': self.segment.to_dict() if self.segment else None,
-            'type': self.type.to_dict() if self.type else None,
-            'subtype': self.subtype.to_dict() if self.subtype else None,
-            'primary': self.primary,
-            'links': self.links,
-        }
+    def __str__(self):
+        return str(self.type)
 
+    # Hypothetical async method to fetch additional details
     async def fetch_additional_details(self, api_client):
         """Asynchronously fetch additional classification details."""
-        details_url = self.links.get('details')
+        # This method is hypothetical and assumes there's a relevant URL in self.links
+        details_url = self.links.get('details')  # Assuming 'details' is a key in links
         if details_url:
-            additional_details = await api_client.get_url(details_url)
-            # Process and integrate additional_details into the Classification instance
+            async with api_client.session.get(details_url) as response:
+                details_json = await response.json()
+                # Process details_json as needed
+
+class EventClassification:
+    """Classification as it's represented in event search results"""
+    def __init__(self, genre=None, subgenre=None, segment=None, classification_type=None, classification_subtype=None, primary=None, links=None):
+        self.genre = genre
+        self.subgenre = subgenre
+        self.segment = segment
+        self.type = classification_type
+        self.subtype = classification_subtype
+        self.primary = primary
+        self.links = links
+
+    @staticmethod
+    def from_json(json_obj):
+        ec = EventClassification()
+        ec.primary = json_obj.get('primary')
+
+        if 'segment' in json_obj:
+            ec.segment = Segment.from_json(json_obj['segment'])
+
+        if 'genre' in json_obj:
+            ec.genre = Genre.from_json(json_obj['genre'])
+
+        if 'subGenre' in json_obj:
+            ec.subgenre = SubGenre.from_json(json_obj['subGenre'])
+
+        if 'type' in json_obj:
+            ec.type = ClassificationType(json_obj['type']['id'], json_obj['type']['name'])
+
+        if 'subType' in json_obj:
+            ec.subtype = ClassificationSubType(json_obj['subType']['id'], json_obj['subType']['name'])
+
+        _assign_links(ec, json_obj)
+        return ec
+
+    def __str__(self):
+        return f"Segment: {self.segment} / Genre: {self.genre} / Subgenre: {self.subgenre} / Type: {self.type} / Subtype: {self.subtype}"
+
 
 class ClassificationType:
     def __init__(self, type_id=None, type_name=None, subtypes=None):
         self.id = type_id
         self.name = type_name
         self.subtypes = subtypes
 
-    @staticmethod
-    def from_json(json_obj):
-        return ClassificationType(
-            type_id=json_obj.get('id'),
-            type_name=json_obj.get('name')
-        )
-
-    def to_dict(self):
-        """Convert the ClassificationType object to a dictionary for serialization"""
-        return {
-            'id': self.id,
-            'name': self.name,
-        }
-
     def __str__(self):
         return self.name if self.name is not None else 'Unknown'
 
+# No changes needed here unless dynamic fetching of subtype details becomes necessary
+
 class ClassificationSubType:
     def __init__(self, type_id=None, type_name=None):
         self.id = type_id
         self.name = type_name
 
-    @staticmethod
-    def from_json(json_obj):
-        return ClassificationSubType(
-            type_id=json_obj.get('id'),
-            type_name=json_obj.get('name')
-        )
-
-    def to_dict(self):
-        """Convert the ClassificationSubType object to a dictionary for serialization"""
-        return {
-            'id': self.id,
-            'name': self.name,
-        }
-
     def __str__(self):
         return self.name if self.name is not None else 'Unknown'
 
+# Similar to ClassificationType, asynchronous behavior might be added for dynamic data fetching
+
 class Segment:
     def __init__(self, segment_id=None, segment_name=None, genres=None, links=None):
         self.id = segment_id
         self.name = segment_name
-        self.genres = genres or []
-        self.links = links or {}
+        self.genres = genres  # Could be a list of Genre instances
+        self.links = links
 
     @staticmethod
     def from_json(json_obj):
-        seg = Segment(
-            segment_id=json_obj.get('id'),
-            segment_name=json_obj.get('name'),
-            genres=[Genre.from_json(g) for g in json_obj.get('_embedded', {}).get('genres', [])]
-        )
+        seg = Segment()
+        seg.id = json_obj['id']
+        seg.name = json_obj.get('name')
+        # Processing embedded genres if available
+        if '_embedded' in json_obj:
+            genres = json_obj['_embedded'].get('genres', [])
+            seg.genres = [Genre.from_json(g) for g in genres]
         _assign_links(seg, json_obj)
         return seg
 
-    def to_dict(self):
-        """Convert the Segment object to a dictionary for serialization"""
-        return {
-            'id': self.id,
-            'name': self.name,
-            'genres': [g.to_dict() for g in self.genres],
-            'links': self.links,
-        }
-
     def __str__(self):
         return self.name if self.name is not None else 'Unknown'
 
+# Could integrate asynchronous methods if genres require fetching additional details
+
 class Genre:
     def __init__(self, genre_id=None, genre_name=None, subgenres=None, links=None):
         self.id = genre_id
         self.name = genre_name
-        self.subgenres = subgenres or []
-        self.links = links or {}
+        self.subgenres = subgenres  # Could be a list of SubGenre instances
+        self.links = links
 
     @staticmethod
     def from_json(json_obj):
-        g = Genre(
-            genre_id=json_obj.get('id'),
-            genre_name=json_obj.get('name'),
-            subgenres=[SubGenre.from_json(sg) for sg in json_obj.get('_embedded', {}).get('subgenres', [])]
-        )
+        g = Genre()
+        g.id = json_obj.get('id')
+        g.name = json_obj.get('name')
+        if '_embedded' in json_obj:
+            subgenres = json_obj['_embedded'].get('subgenres', [])
+            g.subgenres = [SubGenre.from_json(sg) for sg in subgenres]
         _assign_links(g, json_obj)
         return g
 
-    def to_dict(self):
-        """Convert the Genre object to a dictionary for serialization"""
-        return {
-            'id': self.id,
-            'name': self.name,
-            'subgenres': [sg.to_dict() for sg in self.subgenres],
-            'links': self.links,
-        }
-
     def __str__(self):
         return self.name if self.name is not None else 'Unknown'
 
+# Asynchronous enhancements could be added for dynamic subgenre data fetching
+
 class SubGenre:
     def __init__(self, subgenre_id=None, subgenre_name=None, links=None):
         self.id = subgenre_id
         self.name = subgenre_name
-        self.links = links or {}
+        self.links = links
 
     @staticmethod
     def from_json(json_obj):
-        sg = SubGenre(
-            subgenre_id=json_obj.get('id'),
-            subgenre_name=json_obj.get('name')
-        )
+        sg = SubGenre()
+        sg.id = json_obj['id']
+        sg.name = json_obj['name']
         _assign_links(sg, json_obj)
         return sg
 
-    def to_dict(self):
-        """Convert the SubGenre object to a dictionary for serialization"""
-        return {
-            'id': self.id,
-            'name': self.name,
-            'links': self.links,
-        }
-
     def __str__(self):
         return self.name if self.name is not None else 'Unknown'
+
+# Example async usage to fetch and process event details
+async def main():
+    event = Event.from_json({'id': '123', 'name': 'Sample Event', 'links': {'self': 'http://example.com/event/123'}})
+    await event.fetch_additional_details()
+
+if __name__ == '__main__':
+    import asyncio
+    asyncio.run(main())
```

### Comparing `tmticket-0.2.15/pytmtickets/query.py` & `tmticket-0.2.2/tmticket/query.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 """Classes to handle API queries/searches"""
-import logging
-from typing import Any, Dict, List, Type, Optional
-from .model import Venue, Event, Attraction, Classification
-
-log = logging.getLogger(__name__)
+import aiohttp
+from tmticket.model import Venue, Event, Attraction, Classification
 
 class BaseQuery:
     """Base query/parent class for specific search types."""
     attr_map = {
         'start_date_time': 'startDateTime',
         'end_date_time': 'endDateTime',
         'onsale_start_date_time': 'onsaleStartDateTime',
@@ -33,88 +30,105 @@
         'page': 'page',
         'size': 'size',
         'locale': 'locale',
         'latlong': 'latlong',
         'radius': 'radius'
     }
 
-    def __init__(self, api_client, method: str, model: Type[Any]):
+    def __init__(self, api_client, method, model):
         self.api_client = api_client
         self.method = method
         self.model = model
 
-    async def _get(self, **kwargs: Any) -> List[Any]:
+    async def __get(self, **kwargs):
+        """Asynchronously sends final request to `ApiClient`"""
+        async with aiohttp.ClientSession() as session:
+            async with session.get(f"{self.api_client.url}/{self.method}", params={**self.api_client.api_key, **kwargs}) as response:
+                return await response.json()
+
+    async def _get(self, keyword=None, entity_id=None, sort=None, include_test=None, page=None, size=None, locale=None, **kwargs):
         """Asynchronously handles basic API search request"""
-        params = self._search_params(**kwargs)
-        url = f"{self.api_client.url}/{self.method}.json"
-        async with self.api_client.session.get(url, params={**self.api_client.api_key, **params}) as response:
-            response.raise_for_status()
-            data = await response.json()
-            if not isinstance(data, dict) or '_embedded' not in data:
-                log.error(f"Unexpected response format: {data}")
-                raise ApiException("Unexpected response format")
-            return [self.model.from_json(item) for item in data.get('_embedded', {}).get(self.method, [])]
+        search_args = {
+            'keyword': keyword,
+            'id': entity_id,
+            'sort': sort,
+            'include_test': include_test,
+            'page': page,
+            'size': size,
+            'locale': locale,
+            **kwargs
+        }
+        params = self._search_params(**search_args)
+        return await self.__get(**params)
 
-    async def by_id(self, entity_id: str) -> Any:
+    async def by_id(self, entity_id):
         """Asynchronously get a specific object by its ID"""
-        response = await self._get(id=entity_id)
-        if response:
-            return response[0]
-        else:
-            log.error(f"Entity with ID {entity_id} not found")
-            raise ApiException(f"Entity with ID {entity_id} not found")
+        return await self._get(entity_id=entity_id)
 
-    def _search_params(self, **kwargs: Any) -> Dict[str, Any]:
+    def _search_params(self, **kwargs):
         """Maps parameter names to API-friendly parameters"""
-        return {self.attr_map.get(k, k): v for k, v in kwargs.items() if v is not None}
+        kw_map = {}
+        for k, v in kwargs.items():
+            api_key = self.attr_map.get(k)
+            if api_key:
+                kw_map[api_key] = v
+            else:
+                kw_map[k] = v
+        return {k: v for k, v in kw_map.items() if v is not None}
 
 class AttractionQuery(BaseQuery):
     def __init__(self, api_client):
         super().__init__(api_client, 'attractions', Attraction)
 
-    async def find(self, **kwargs: Any) -> List[Attraction]:
+    async def find(self, **kwargs):
         return await self._get(**kwargs)
 
 class ClassificationQuery(BaseQuery):
     def __init__(self, api_client):
         super().__init__(api_client, 'classifications', Classification)
 
-    async def find(self, **kwargs: Any) -> List[Classification]:
-        return await self._get(**kwargs)
 
-    async def segment_by_id(self, segment_id: str) -> Optional[Any]:
-        """Return a `Segment` matching this ID"""
-        classification = await self.by_id(segment_id)
-        return classification.segment if classification else None
-
-    async def genre_by_id(self, genre_id: str) -> Optional[Any]:
-        """Return a `Genre` matching this ID"""
-        classification = await self.by_id(genre_id)
-        if classification and classification.segment:
-            for genre in classification.segment.genres:
+    def segment_by_id(self, segment_id):
+        """Return a ``Segment`` matching this ID"""
+        return self.by_id(segment_id).segment
+
+    def genre_by_id(self, genre_id):
+        """Return a ``Genre`` matching this ID"""
+        genre = None
+        resp = self.by_id(genre_id)
+        if resp.segment:
+            for genre in resp.segment.genres:
                 if genre.id == genre_id:
-                    return genre
-        return None
+                    genre = genre
+        return genre
 
-    async def subgenre_by_id(self, subgenre_id: str) -> Optional[Any]:
-        """Return a `SubGenre` matching this ID"""
-        classification = await self.by_id(subgenre_id)
-        if classification and classification.segment:
-            for genre in classification.segment.genres:
-                for subgenre in genre.subgenres:
-                    if subgenre.id == subgenre_id:
-                        return subgenre
-        return None
+    def subgenre_by_id(self, subgenre_id):
+        """Return a ``SubGenre`` matching this ID"""
+        subgenre = None
+        segment = self.by_id(subgenre_id).segment
+        if segment:
+            subgenres = [
+                subg for genre in segment.genres
+                for subg in genre.subgenres
+            ]
+            for subg in subgenres:
+                if subg.id == subgenre_id:
+                    subgenre = subg
+        return subgenre
+
+
+    async def find(self, **kwargs):
+        return await self._get(**kwargs)
 
 class EventQuery(BaseQuery):
     def __init__(self, api_client):
         super().__init__(api_client, 'events', Event)
 
-    async def find(self, **kwargs: Any) -> List[Event]:
+    async def find(self, **kwargs):
         return await self._get(**kwargs)
 
 class VenueQuery(BaseQuery):
     def __init__(self, api_client):
         super().__init__(api_client, 'venues', Venue)
 
-    async def find(self, **kwargs: Any) -> List[Venue]:
+    async def find(self, **kwargs):
         return await self._get(**kwargs)
```

