## Put comments here that give an overall description of what your
## functions do

## Write a short comment describing this function



## mean -> Inverse
## setmean -> setInverse
## getmean -> getInverse

## function to create matrix to cache its inverse
makeCacheMatrix <- function(x = matrix()) {

## initializing the inverse
m <- NULL

## setting up the matrix
set <- function(y) {
    x <<- y
    m <<- NULL
}

## getting the matrix
get <- function() x

## inverting the matrix
setInverse <- function(Inverse) m <<- Inverse

## getting the inverse of matrix
getInverse <- function() m

## returning the list
list(set = set, get = get,
    setInverse = setInverse,
    getInverse = getInverse)
}


## Write a short comment describing this function

## function to compute inverse square matrix
cacheSolve <- function(x, ...) {
        ## Return a matrix that is the inverse of 'x'
        m <- x$getInverse()
        if(!is.null(m)) {
            message("getting cached data")
            return(m)
        }

## getting matrix from object
        data <- x$get()
        
## calculating inverse matrix
        m <- solve(data, ...)
        x$setInverse(m)
        
## returning computed inverse matrix
        m
}
