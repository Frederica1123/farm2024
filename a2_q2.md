### a2_q2_v3 ###
a2_q2 <- function(n) {
  result <- list()
  result$power_xy <- n[["x"]] ** n[["y"]]
  result$power_yx <- n[["y"]] ** n[["x"]]
  result$repeat_x_times <- paste0(replicate(n[["x"]], "x"), collapse = "")
  result$repeat_y_times <- paste0(replicate(n[["y"]], n["y"]), collapse = "")
  result$xth_alphabet_repeat_y_times <- paste0(replicate(n[["y"]], letters[n[["x"]]]), collapse = "")
  return(result)
}
