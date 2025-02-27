data <- c(11, 13, 13, 15, 15, 16, 19, 20, 20, 20, 21, 21, 22, 23, 24, 30, 40, 45, 45, 45, 71, 72, 73, 75)

bins <- split(data, cut(data, 3, include.lowest = TRUE))

bin_mean <- lapply(bins, mean)

bin_median <- lapply(bins, median)

bin_boundaries <- lapply(bins, function(x) ifelse(x < median(x), min(x), max(x)))

list(mean = bin_mean, median = bin_median, boundaries = bin_boundaries)
