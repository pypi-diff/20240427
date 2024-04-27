# Comparing `tmp/radinNFP-2.4.3-py3-none-any.whl.zip` & `tmp/radinNFP-2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 9613 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat    78665 b- defN 24-Feb-14 07:48 radinNFP/__init__.py
--rw-rw-rw-  2.0 fat      284 b- defN 24-Feb-14 07:53 radinNFP-2.4.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Feb-14 07:53 radinNFP-2.4.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-Feb-14 07:53 radinNFP-2.4.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      378 b- defN 24-Feb-14 07:53 radinNFP-2.4.3.dist-info/RECORD
-5 files, 79428 bytes uncompressed, 8907 bytes compressed:  88.8%
+Zip file size: 8773 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat    65975 b- defN 24-Apr-27 06:20 radinNFP/__init__.py
+-rw-rw-rw-  2.0 fat      282 b- defN 24-Apr-27 06:24 radinNFP-2.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-27 06:24 radinNFP-2.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-Apr-27 06:24 radinNFP-2.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      370 b- defN 24-Apr-27 06:24 radinNFP-2.5.dist-info/RECORD
+5 files, 66728 bytes uncompressed, 8083 bytes compressed:  87.9%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: radinNFP/__init__.py
 Comment: 
 
-Filename: radinNFP-2.4.3.dist-info/METADATA
+Filename: radinNFP-2.5.dist-info/METADATA
 Comment: 
 
-Filename: radinNFP-2.4.3.dist-info/WHEEL
+Filename: radinNFP-2.5.dist-info/WHEEL
 Comment: 
 
-Filename: radinNFP-2.4.3.dist-info/top_level.txt
+Filename: radinNFP-2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: radinNFP-2.4.3.dist-info/RECORD
+Filename: radinNFP-2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## radinNFP/__init__.py

```diff
@@ -32,36 +32,29 @@
         if isinstance(other, Line):
             return (self.startPoint == other.startPoint and
                     self.endPoint == other.endPoint and
                     self.slope == other.slope and
                     self.idx == other.idx)
         return False
     
-    def line_in_list(self,lList):
-        
-        for line in lList:
-            if self.idx == line:
-                return True
-            return False
-        
     def __hash__(self):
         
         return hash((self.startPoint, self.endPoint, self.slope,self.idx))
     
     def is_startPoint(self, point):
         
         return point.x == self.startPoint.x and point.y == self.startPoint.y
 
     def is_endPoint(self, point):
         
         return point.x == self.endPoint.x and point.y == self.endPoint.y
     
 class NFP(object):
     def __init__(self, outer, supA = None, supB = None, holeA = None, holeB = None):
-        self.outer = outer,
+        self.outer = outer
         self.supA = [] if supA is None else supA
         self.supB = [] if supB is None else supB
         self.holeA = [] if holeA is None else holeA
         self.holeB = [] if holeB is None else holeB
         
 def angle_finder(line1,line2):
     
@@ -267,15 +260,14 @@
                 pTvec = Line(point[4],Point(point[4].x + Tvec[0],point[4].y + Tvec[1]),(((point[4].y + Tvec[1]) - point[4].y)/((point[4].x + Tvec[0]) - point[4].x)) if ((point[4].x + Tvec[0]) - point[4].x) != 0 else None,1)
                 if ((left_or_right(pTvec,translateV.endPoint) == "right") or (left_or_right(pTvec,translateV.endPoint) == "parallel")):
                     pass
                 else:
                     return False
 
 def fractionalize(polygon):
-    
     finalPolygon = []
     finalPolygon.append([[Fraction(x),Fraction(y)] for x,y in polygon[0]])
     for p in polygon[1:]:
         finalPolygon.append([[Fraction(x),Fraction(y)] for x,y in p])
     return finalPolygon
 
 def lowest_key(polygon):
@@ -439,15 +431,15 @@
     for edge in edges:
         if(not 
            ((((left_or_right(seg1,edge.startPoint) == "left") and (left_or_right(seg1,edge.endPoint) == "left")) and ((left_or_right(seg2,edge.startPoint) == "left") and (left_or_right(seg2,edge.endPoint) == "left"))) 
            or
            (((left_or_right(seg1,edge.startPoint) == "right") and (left_or_right(seg1,edge.endPoint) == "right")) and ((left_or_right(seg2,edge.startPoint) == "right") and (left_or_right(seg2,edge.endPoint) == "right")))
            )):
             filtered_edges.append(edge)
-    return filtered_edges
+    return filtered_edges if (len(filtered_edges) !=0) else edges
 
 def is_point_on_segment(point,line):
     
     min_y=min(line.startPoint.y,line.endPoint.y)
     max_y=max(line.startPoint.y,line.endPoint.y)
     min_x=min(line.startPoint.x,line.endPoint.x)
     max_x=max(line.startPoint.x,line.endPoint.x)
@@ -508,15 +500,15 @@
     if(point1[1] > point2[1]):
         return True
     elif(point1[1] == point2[1] and point1[0] < point2[0]):
         return True
     else:
         return False
 
-def overlapTest(polygonA,polygonB,edgesA,edgesB,point):
+def overlapTest(edgesA,edgesB):
     intersection = []
     for edgeA in edgesA:
         try:
             for edgeB in edgesB:
                 if bounding(edgeA,edgeB):
                     intersect = find_intersection(edgeA,edgeB)
                     if( intersect!= None):
@@ -579,15 +571,15 @@
    
     
     if(len(intersection)==0):
         return True
     else:
         return False
     
-def holeOverlapTest(hole,polygonB,holeEdges,edgesB,point):
+def holeOverlapTest(holeEdges,edgesB):
     intersection = []
     for holeEdge in holeEdges:
         try:
             for edgeB in edgesB:
                 if bounding(holeEdge,edgeB):
                     intersect = find_intersection(holeEdge,edgeB)
                     if( intersect!= None):
@@ -652,17 +644,14 @@
                                                (left_or_right(pEdgeHole,pEdgeB.startPoint) == "left" and left_or_right(holeEdge,pEdgeB.startPoint) == "left")
                                                ):
                                                 intersection.append(intersect)
                                                 raise StopIteration 
         except StopIteration:
             break
    
-    
-    
-   
     if(len(intersection)==0):
         return True
     else:
         return False
 
 def NFP2(startPoint,touchPoint,polygonA,polygonB,edgesA,cond2,cond1=True,touchingEdge=None):
     
@@ -793,15 +782,14 @@
                                 filteredEdgesA = boundry(polygonB2,edgesA,tVec)
                                 filteredEdgesB2 = boundry(polygonA,edgesB2,tVec)
                                 edgesB2 = [Line(Point(a[0],a[1]),Point(b[0],b[1]),slope(a,b),idx)  for idx, (a, b) in enumerate(zip(polygonB2, polygonB2[1:] + [polygonB2[0]]))]
                                 if(overlapTest(polygonA,polygonB2,edgesA,edgesB2,touchPoint)):
                                     
                                     if(lowest_key(polygonB2) not in nfpPointList2 ):
                                         inner_nfp = NFP2(startPoint,touchPoint,polygonA,polygonB2,edgesA,cond2,cond1,l)
-                                        # #print(f"inner NFP:{inner_nfp}")
                                         nfpList.append(inner_nfp[0])
                                         navigatedA = inner_nfp[1]
                                         navigatedB.extend(inner_nfp[2])
                                         
                                         nfpPointList2.extend(inner_nfp[0])
                                         raise StopIteration
                                     else:
@@ -1038,15 +1026,14 @@
         vE = edgeRemover(next_info,visitedEdgesA,visitedEdgesB,edgesA,edgesB2)
         visitedEdgesA = vE[0]
         y += 1 
     return (nfp,visitedEdgesA)
 
 
 def nfpSupHole2(polygonA,polygonB,remainedEdgesA,nfpPointList):
-    
     navigatedA = []
     nfpList = []
     edgesA = [Line(Point(a[0],a[1]),Point(b[0],b[1]),slope(a,b),idx)  for idx, (a, b) in enumerate(zip(polygonA, polygonA[1:] + [polygonA[0]]))] 
     for edge in remainedEdgesA:
         mPoint = (edge.startPoint.x,edge.startPoint.y)
         for indx,point in enumerate(polygonB):
             if( edge.idx not in navigatedA):
@@ -1103,156 +1090,21 @@
                                     tVec = (tVec[0] - (-t1[0]),tVec[1] - (-t1[1]))
                                     touchPoint = (touchPoint[0] + (-t1[0]), touchPoint[1] + (-t1[1]))
                                     startPoint = touchPoint
                             except StopIteration:
                                 break
     return nfpList
                   
-def NFPHole(startPoint,touchPoint,polygonA,polygonB,edgesA,cond2,cond1=True,touchingEdge=None):
-    
-    polygonB2 = polygonB[:]
-    diff_vec = (touchPoint[0]- startPoint[0], touchPoint[1] - startPoint[1])
-    polygonB2= [[x - diff_vec[0], y - diff_vec[1]] for x,y in polygonB2]
-    y=0
-    
-    nfp = []
-    x=(None,None)
-    wCond = lowest_key(polygonB2)
-    point = Point(startPoint[0],startPoint[1])
-   
-    edgesB = [Line(Point(a[0],a[1]),Point(b[0],b[1]),slope(a,b),idx)  for idx, (a, b) in enumerate(zip(polygonB2, polygonB2[1:] + [polygonB2[0]]))] 
-    nextTv =  tVectorFinder(point,edgesA,edgesB,cond1,cond2,touchingEdge)[0]
-    if(cond2 == True):
-        edgeA= touchingEdge
-    else:
-        edgeA= next(filter(lambda e: e.is_startPoint(point)  , edgesA))
-    edgeB= next(filter(lambda e: e.is_startPoint(point)  , edgesB))
-   
-    p = Point(point.x + nextTv[0],point.y + nextTv[1])
-    if((edgeA.endPoint.x - edgeA.startPoint.x) == nextTv[0] and (edgeA.endPoint.x - edgeA.startPoint.x) == nextTv[1]):
-        next_info = [point,edgeA,True,False,p,polygonA.index([point.x,point.y])]
-    else:
-        next_info = [point,edgeB,False,True,p,polygonB2.index([point.x,point.y])]
-        
-    visitedEdgesA =set() 
-    visitedEdgesB =set() 
-    vE = edgeRemover(next_info,visitedEdgesA,visitedEdgesB,edgesA,edgesB)
-     
-    visitedEdgesB = vE[1] 
-    c = 0
-    while (((x[0] != wCond[0]) or(x[1] != wCond[1]) or y <2) and c!=2):
-        edgesB = [Line(Point(a[0],a[1]),Point(b[0],b[1]),slope(a,b),idx)  for idx, (a, b) in enumerate(zip(polygonB2, polygonB2[1:] + [polygonB2[0]]))] 
-
-        filteredEdgesA = boundry(polygonB2,edgesA,nextTv)
-        filteredEdgesB = boundry(polygonA,edgesB,(-nextTv[0],-nextTv[1]))
-        t1 = holeTrimmer(polygonB2,filteredEdgesA,nextTv,edgesA)
-        t2 = holeTrimmer(polygonA,filteredEdgesB,(-t1[0],-t1[1]),edgesB)
-
-        polygonB2 = [[x + (-t2[0]), y + (-t2[1])] for x, y in polygonB2]
-        trim1 = trimFun(polygonB2,filteredEdgesA,(-t2[0],-t2[1]),True)
-        edgesB2 = [Line(Point(a[0],a[1]),Point(b[0],b[1]),slope(a,b), idx)  for idx, (a, b) in enumerate(zip(polygonB2, polygonB2[1:] + [polygonB2[0]]))]
-        filteredEdgesB2 = boundry(polygonA,edgesB2,(-t2[0],-t2[1]))
-        trim2 = trimFun(polygonA,filteredEdgesB2,t2,False)
-        vecList = []
-        if(nfp.__contains__(lowest_key(polygonB2))):
-            c +=1
-        nfp.append(lowest_key(polygonB2))
-
-        idealTV=[]
-        trimResults = trim1 + trim2
-    
-        for info in trimResults:
-            possibleNextVector = tVectorFinder(info[4],edgesA,edgesB2,info[2],info[3],info[1])[0]
-            vecList.append(possibleNextVector)
-        for j,vector in enumerate(vecList):
-            if(feasibleTV(edgesA,edgesB2,vector,trimResults) == False):
-                pass
-            else:
-                idealTV.append((vector,trimResults[j][4],trimResults[j]))
-        distanceL = []
-        if(len(idealTV) == 0 ):
-            break
-        for l in idealTV:
-            tvec = Line(point,Point(point.x + (-t2[0]/2),point.y + (-t2[1]/2)),5,1)
-            distanceL.append(distance(tvec,l[1]))
-        index = distanceL.index(min(distanceL))
-        next_info = idealTV[index][2]
-        nextTv = idealTV[index][0]
-        point = idealTV[index][1]
-        x = nfp[-1]
-        vE = edgeRemover(next_info,visitedEdgesA,visitedEdgesB,edgesA,edgesB2)
-        visitedEdgesB = vE[1]
-        y += 1 
-    return (nfp,visitedEdgesB)
 
-def nfpSupHole(polygonA,polygonB,remainedEdgesB,nfpPointList,edgesA):
-   
-    navigated = []
-    nfpList = []
-    for edge in remainedEdgesB:
-        sPoint = (edge.startPoint.x,edge.startPoint.y)
-        for idx,point in enumerate(polygonA):
-            if( edge.idx not in navigated):
-                polygonB2 = polygonB[:]
-                difference_vec = (point[0] - sPoint[0],point[1] - sPoint[1])
-                polygonB2 = [[x + difference_vec[0], y + difference_vec[1]] for [x,y] in polygonB2]
-                edgesB2 = [Line(Point(a[0],a[1]),Point(b[0],b[1]),slope(a,b),idx)  for idx, (a, b) in enumerate(zip(polygonB2, polygonB2[1:] + [polygonB2[0]]))] 
-                startingEdgeA = edgesA[idx]
-                endingEdgeA = edgesA[idx - 1]
-                
-                if(left_or_right(edgesB2[edge.idx],startingEdgeA.endPoint) == "left" or left_or_right(edgesB2[edge.idx],endingEdgeA.startPoint) == "left"):
-                    pass
-                
-                else:
-                        tVec = (edge.startPoint.x - edge.endPoint.x, edge.startPoint.y - edge.endPoint.y)
-                        if(find_intersectionSup(edgesB2[edge.idx],startingEdgeA) or ((find_intersectionSup(edgesB2[edge.idx],endingEdgeA)))):
-                            pass
-                        else:
-                            orgtVec = tVec
-                            cond1 = True
-                            cond2 = False
-                            l = None
-                            startPoint = point
-                            touchPoint = startPoint
-                            while(vectorDiff(orgtVec,tVec) != orgtVec):    
-                                try:
-                                    edgesB2 = [Line(Point(a[0],a[1]),Point(b[0],b[1]),slope(a,b),idx)  for idx, (a, b) in enumerate(zip(polygonB2, polygonB2[1:] + [polygonB2[0]]))] 
-                                    filteredEdgesA = boundry(polygonB2,edgesA,tVec)
-                                    filteredEdgesB2 = boundry(polygonA,edgesB2,tVec)
-                                    if(holeOverlapTest(polygonB2,polygonA,edgesB2,edgesA,touchPoint)):
-                                        if(lowest_key(polygonB2) not in nfpPointList ):
-                                            inner_nfp = NFPHole(startPoint,touchPoint,polygonA,polygonB2,edgesA,cond2,cond1,l)
-                                            nfpList.append(inner_nfp[0])
-                                            
-                                            navigated = inner_nfp[1]
-                                            nfpPointList.extend(inner_nfp[0])
-                                            raise StopIteration
-                                        else:
-                                            break
-                                    else:
-                                        t = trimmerSup(polygonB2,filteredEdgesA,tVec)
-                                        t1 = trimmerSup(polygonA,filteredEdgesB2,(-t[0],-t[1]))
-                                        polygonB2 = [[x + (-t1[0]), y + (-t1[1])] for x, y in polygonB2]
-                                        cond2 = True
-                                        cond1 = False
-                                        edgesB2 = [Line(Point(a[0],a[1]),Point(b[0],b[1]),slope(a,b),idx)  for idx, (a, b) in enumerate(zip(polygonB2, polygonB2[1:] + [polygonB2[0]]))] 
-                                        l = edgesB2[edge.idx]
-                                        tVec = (tVec[0] - (-t1[0]),tVec[1] - (-t1[1]))
-                                        touchPoint = (touchPoint[0] + (-t1[0]), touchPoint[1] + (-t1[1]))
-                                        startPoint = touchPoint
-                                except StopIteration:
-                                    break
-    return nfpList
 
 def outerNFP(startPoint,touchPoint,polygonA,polygonB,edgesA):
     
     polygonB2 = polygonB[:]
     diff_vec = (touchPoint[0]- startPoint[0], touchPoint[1] - startPoint[1])
     polygonB2= [[x - diff_vec[0], y - diff_vec[1]] for x,y in polygonB2]
-    nfp = []
     y=0
     x=(None,None)
     wCond = lowest_key(polygonB2)
     point = Point(startPoint[0],startPoint[1])
     edgesB = [Line(Point(a[0],a[1]),Point(b[0],b[1]),slope(a,b),idx)  for idx, (a, b) in enumerate(zip(polygonB2, polygonB2[1:] + [polygonB2[0]]))] 
     nextTv =  tVectorFinder(point,edgesA,edgesB)[0]
     edgeA= next(filter(lambda e: e.is_startPoint(point)  , edgesA))
@@ -1263,15 +1115,14 @@
     else:
         next_info = [point,edgeB,False,False,p,polygonB2.index([point.x,point.y])]
     visitedEdgesA =set() 
     visitedEdgesB = set()
     vE = edgeRemover(next_info,visitedEdgesA,visitedEdgesB,edgesA,edgesB)
     visitedEdgesA = vE[0]
     visitedEdgesB = vE[1]
-        
     
     while (((x[0] != wCond[0]) or(x[1] != wCond[1]) or y <2)):
         edgesB = [Line(Point(a[0],a[1]),Point(b[0],b[1]),slope(a,b),idx)  for idx, (a, b) in enumerate(zip(polygonB2, polygonB2[1:] + [polygonB2[0]]))] 
         filteredEdgesA = boundry(polygonB2,edgesA,nextTv)
         filteredEdgesB = boundry(polygonA,edgesB,(-nextTv[0],-nextTv[1]))
         t1 = trimmer(polygonB2,filteredEdgesA,nextTv)
         t2 = trimmer(polygonA,filteredEdgesB,(-t1[0],-t1[1]))
@@ -1306,19 +1157,20 @@
         index = distanceL.index(min(distanceL))
         next_info = idealTV[index][2]
         
         nextTv = idealTV[index][0]
         point = idealTV[index][1]
         x = nfp[-1] 
         
+        
         vE = edgeRemover(next_info,visitedEdgesA,visitedEdgesB,edgesA,edgesB2)
         visitedEdgesA = vE[0]
         visitedEdgesB = vE[1]
         y += 1
-       
+    
     remainedEdgeA = edgesA[:]
     
     for idx in visitedEdgesA:
         remainedEdgeA.remove(edgesA[idx])
     return (nfp,remainedEdgeA,visitedEdgesB)
 
 #calculating the bounding box and it's height and length
@@ -1338,139 +1190,47 @@
 
     # Calculate length and height of bounding box
     length = max_x - min_x
     height = max_y - min_y
 
     return [length, height]
 
+    
 def finalNFP(polygonA,polygonB):
-
     edgesA = None
     a_RefPoint = None
-    edgesOrgB = None
     b_highPoint = None
-    
-    
+
     if(len(polygonA[0]) > 2 ):
         polygonA = fractionalize(polygonA)
         edgesA = [Line(Point(a[0],a[1]),Point(b[0],b[1]),slope(a,b),idx)  for idx, (a, b) in enumerate(zip(polygonA[0], polygonA[0][1:] + [polygonA[0][0]]))]
         a_RefPoint = lowest_key(polygonA[0])
     else: 
         polygonA = [[Fraction(x),Fraction(y)] for x,y in polygonA]
         edgesA = [Line(Point(a[0],a[1]),Point(b[0],b[1]),slope(a,b),idx)  for idx, (a, b) in enumerate(zip(polygonA, polygonA[1:] + [polygonA[0]]))]
         a_RefPoint = lowest_key(polygonA)
     
     if(len(polygonB[0]) > 2 ):
         polygonB = fractionalize(polygonB)
-        edgesOrgB = [Line(Point(a[0],a[1]),Point(b[0],b[1]),slope(a,b),idx)  for idx, (a, b) in enumerate(zip(polygonB[0], polygonB[0][1:] + [polygonB[0][0]]))]
         b_highPoint = highest_key(polygonB[0])
     else: 
         polygonB = [[Fraction(x),Fraction(y)] for x,y in polygonB]
-        edgesOrgB = [Line(Point(a[0],a[1]),Point(b[0],b[1]),slope(a,b),idx)  for idx, (a, b) in enumerate(zip(polygonB, polygonB[1:] + [polygonB[0]]))]
         b_highPoint = highest_key(polygonB)
     outerNfp=[]
-
     if(len(polygonA[0]) > 2 and len(polygonB[0]) > 2 ):
         outerNfp = outerNFP(a_RefPoint,b_highPoint,polygonA[0],polygonB[0],edgesA)
     elif(len(polygonA[0]) > 2 ):
         outerNfp = outerNFP(a_RefPoint,b_highPoint,polygonA[0],polygonB,edgesA)
     elif(len(polygonB[0]) > 2 ):
         outerNfp = outerNFP(a_RefPoint,b_highPoint,polygonA,polygonB[0],edgesA)
     else:
         outerNfp = outerNFP(a_RefPoint,b_highPoint,polygonA,polygonB,edgesA)
 
     res = NFP(outerNfp[0])
     
-    remainedEdge  = edgesOrgB[:]
-    remainedEdgesA = outerNfp[1]
-    remainedEdgesB = outerNfp[2]
-    visitedB = None
-
- 
-    if(len(remainedEdgesA) > 0):
-        if(len(polygonA[0]) > 2):
-            if(len(polygonB[0]) > 2 ):
-                innerNfp = nfpSup(polygonA[0],polygonB[0],remainedEdgesA,outerNfp[0])
-                visitedB = set(innerNfp[1])
-                for supNfp in innerNfp[0]:
-                    if(len(supNfp) == 0):
-                        pass
-                    else:
-                        res.supA.append(supNfp)                    
-            else:
-                innerNfp = nfpSup(polygonA[0],polygonB,remainedEdgesA,outerNfp[0])
-                visitedB = set(innerNfp[1])
-                for supNfp in innerNfp[0]:
-                    if(len(supNfp) == 0):
-                        pass
-                    else:
-                        res.supA.append(supNfp)
-        else:
-            if(len(polygonB[0]) > 2 ):
-                innerNfp = nfpSup(polygonA,polygonB[0],remainedEdgesA,outerNfp[0])
-                visitedB = set(innerNfp[1])
-                for supNfp in innerNfp[0]:
-                    if(len(supNfp) == 0):
-                        pass
-                    else:
-                        res.supA.append(supNfp)
-            else:
-                innerNfp = nfpSup(polygonA,polygonB,remainedEdgesA,outerNfp[0])
-                visitedB = set(innerNfp[1])
-                for supNfp in innerNfp[0]:
-                    if(len(supNfp) == 0):
-                        pass
-                    else:
-                        res.supA.append(supNfp)
-    
-
-    vistededgesB = None
-    if((visitedB is not None) and (remainedEdgesB is not None)):
-        vistededgesB = remainedEdgesB | visitedB
-    elif(visitedB is None): 
-        vistededgesB = remainedEdgesB
-    elif(remainedEdgesB is None):
-        vistededgesB = visitedB
-    if(vistededgesB is not None):
-        for idx in vistededgesB:
-            remainedEdge.remove(edgesOrgB[idx])
-    
-    if(len(remainedEdge) > 0):
-        if(len(polygonA[0]) > 2):
-            if(len(polygonB[0]) > 2 ):
-                innerNfp2 = nfpSupB2A(polygonA[0],polygonB[0],remainedEdge,outerNfp[0],edgesA)
-                for supNfp in innerNfp2:
-                    if(len(supNfp) == 0):
-                        pass
-                    else:
-                        res.supB.append(supNfp)
-            else:
-                innerNfp2 = nfpSupB2A(polygonA[0],polygonB,remainedEdge,outerNfp[0],edgesA)
-                for supNfp in innerNfp2:
-                    if(len(supNfp) == 0):
-                        pass
-                    else:
-                        res.supB.append(supNfp)
-        else:
-            if(len(polygonB[0]) > 2 ):
-                innerNfp2 = nfpSupB2A(polygonA,polygonB[0],remainedEdge,outerNfp[0],edgesA)
-                for supNfp in innerNfp2:
-                    if(len(supNfp) == 0):
-                        pass
-                    else:
-                        res.supB.append(supNfp)
-            else:
-                innerNfp2 = nfpSupB2A(polygonA,polygonB,remainedEdge,outerNfp[0],edgesA)
-                for supNfp in innerNfp2:
-                    if(len(supNfp) == 0):
-                        pass
-                    else:
-                        res.supB.append(supNfp)
-    
-    innerPNFPs = []
     if(len(polygonA[0]) > 2):
         for innerP in polygonA[1:]:
             innerEdges = [Line(Point(a[0],a[1]),Point(b[0],b[1]),slope(a,b),idx)  for idx, (a, b) in enumerate(zip(innerP, innerP[1:] + [innerP[0]]))]
             innerPBB = calculate_bounding_box_dimensions(innerP)
             if(len(polygonB[0])>2):
                 polygonBBB = calculate_bounding_box_dimensions(polygonB[0])
                 if(innerPBB[0]>= polygonBBB[0] and innerPBB[1] >= polygonBBB[1]):
@@ -1486,31 +1246,8 @@
                     lp = nfpSupHole2(innerP,polygonB,innerEdges,[])
                     for supNfp in lp:
                         if(len(supNfp) == 0):
                             pass
                         else:
                             res.holeA.append(supNfp) 
     
-    
-    if(len(polygonB[0]) > 2):
-        holeNfp= []
-        lowp1= lowest_key(polygonB[0])
-        for innerP in polygonB[1:]:
-            innerPBB = calculate_bounding_box_dimensions(innerP)
-            lowi = lowest_key(innerP)
-            difference = (lowp1[0] - lowi[0], lowp1[1] - lowi[1])
-            innerEdges = [Line(Point(a[0],a[1]),Point(b[0],b[1]),slope(a,b),idx)  for idx, (a, b) in enumerate(zip(innerP, innerP[1:] + [innerP[0]]))]
-            if(len(polygonA[0]) > 2 ):
-                polygonABB = calculate_bounding_box_dimensions(polygonA[0])
-                if(innerPBB[0]>= polygonABB[0] and innerPBB[1] >= polygonABB[1]):
-                    holeNfp = nfpSupHole(polygonA[0],innerP,innerEdges,[],edgesA)
-            else:
-                polygonABB = calculate_bounding_box_dimensions(polygonA)
-                if(innerPBB[0]>= polygonABB[0] and innerPBB[1] >= polygonABB[1]):
-                    holeNfp = nfpSupHole(polygonA,innerP,innerEdges,[],edgesA)
-            for nfp in holeNfp:
-                if(len(nfp) == 0):
-                    pass
-                else:
-                    res.holeB.append([[x[0] + difference[0],x[1] + difference[1]] for x in nfp])
-    
     return res
```

