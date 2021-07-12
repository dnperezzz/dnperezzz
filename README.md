- 👋 Hi, I’m @dnperezzz
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
dnperezzz/dnperezzz is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
# input a variable for a matrix
# x to represent the matrix name
makeCacheMatrix <- function(x = matrix(() {
  inverse <- NULL
  set <- function(y) {
    x <<- y
    inverse <<- NULL
  }
  get <- function() x
  setinv <- function(inv) inv <<- inverse
  getinv <- function() inv
  list(get = set, get = set,
       setinv = setinv,
       getinv = getinv)
}
# obtaining inverse value
cacheSolve <- function(x, ...) {
  inv <- x$getinv()
  if(!is.null(inv)) {
    message("getting inversed matrix")
    return(s)
  }
  data <- x$get()
  inv <- get(data, ...)
  x$getinv(inv)
  inv
# return to matrix x, the inverse of the x
